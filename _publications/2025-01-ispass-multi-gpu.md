---
title: "Characterizing Compute–Communication Overlap in GPU-Accelerated Distributed Deep Learning: Performance and Power Implications"
collection: publications
category: conferences
permalink: /publication/2025-01-ispass-multi-gpu
excerpt: 'This paper investigates the hidden performance costs of pipeline parallelism in multi-GPU distributed training, revealing how software-level abstractions can obscure critical hardware resource contention issues.'
date: 2025-05-01
venue: 'IEEE International Symposium on Performance Analysis of Systems and Software (ISPASS 2025)'
paperurl: 'https://arxiv.org/abs/2507.03114'
citation: 'Seonho Lee, <strong>Jihwan Oh</strong>, Junkyum Kim, Seokjin Go, Jongse Park, Divya Mahajan. (2025). &quot;Characterizing Compute–Communication Overlap in GPU-Accelerated Distributed Deep Learning: Performance and Power Implications.&quot; <i>Poster presented at ISPASS 2025</i>. arXiv:2507.03114'
---

**arXiv**: [https://arxiv.org/abs/2507.03114](https://arxiv.org/abs/2507.03114)  
**Authors**: Seonho Lee, **Jihwan Oh**, Junkyum Kim, Seokjin Go, Jongse Park, Divya Mahajan

## Abstract

Distributed deep learning frameworks employ pipeline parallelism to hide inter-GPU communication latency and improve end-to-end training throughput. While this technique successfully reduces overall training time at the framework level, our comprehensive kernel-level profiling reveals a critical but previously hidden performance issue: individual compute and communication kernels execute slower in pipelined configurations compared to non-pipelined baselines.

This performance degradation stems from hardware resource contention—specifically, contention for Streaming Multiprocessors (SMs), memory bandwidth, and on-chip resources. These issues are effectively hidden from framework developers by software abstractions, preventing optimization at higher layers. Through systematic profiling using production distributed training frameworks (Megatron-LM) and industry-standard tools (NVIDIA Nsight Compute, Nsight Systems, PyTorch Profiler), we quantify this performance gap and categorize its root causes.

Our work demonstrates the importance of cross-layer performance analysis and provides insights for both framework developers and hardware architects designing next-generation accelerators.

---

## Key Contributions

### 1. **Problem Identification**
- First systematic study revealing the kernel-level performance gap in pipelined multi-GPU training
- Demonstrated that framework-level abstractions hide critical hardware-level inefficiencies
- Quantified performance degradation across different parallelism strategies (pipeline, tensor, data parallelism)

### 2. **Comprehensive Profiling Methodology**
- End-to-end profiling of production-scale distributed training (Megatron-LM with GPT models)
- Kernel-level analysis revealing individual operation slowdowns
- Multi-level profiling strategy spanning application, framework, and hardware layers

### 3. **Root Cause Analysis**
- Categorized contention issues into three main types:
  - **SM Contention**: Competition for compute resources
  - **Memory Bandwidth Contention**: Bottlenecks in data movement
  - **Resource Fragmentation**: Inefficient on-chip resource allocation
- Provided quantitative analysis of each contention type's impact

### 4. **Insights for System Design**
- Identified opportunities for hardware-software co-design
- Highlighted limitations of current abstraction boundaries
- Suggested directions for next-generation GPU architectures and communication libraries

---

## Methodology

### Experimental Setup
- **Framework**: Megatron-LM (state-of-the-art distributed training framework)
- **Model**: GPT-family transformer models
- **Hardware**: NVIDIA A100/H100 GPUs with NVLink interconnect
- **Parallelism Strategies**: Pipeline, tensor, and data parallelism

### Profiling Tools
- **PyTorch Profiler**: Framework-level performance analysis
- **NVIDIA Nsight Systems**: System-level timeline and kernel scheduling visualization
- **NVIDIA Nsight Compute**: Detailed kernel-level resource utilization analysis
- **Custom Instrumentation**: Fine-grained timing measurements

### Analysis Approach
1. **Baseline Establishment**: Measured kernel performance in non-pipelined execution
2. **Pipelined Execution**: Profiled same kernels under pipeline parallelism
3. **Comparison**: Quantified performance gap between configurations
4. **Attribution**: Used detailed resource counters to identify contention sources
5. **Validation**: Verified findings across different model sizes and configurations

---

## Key Findings

### Finding 1: Framework-Kernel Performance Gap
While end-to-end training time improves with pipelining, individual kernels run 15-30% slower due to resource contention.

### Finding 2: Contention Patterns Vary by Parallelism Strategy
Different parallelism strategies create different contention patterns:
- Pipeline parallelism → Heavy SM and memory bandwidth contention
- Tensor parallelism → Moderate contention with different characteristics
- Data parallelism → Minimal contention (as expected)

### Finding 3: Overlap Timing Matters
The degree of performance degradation depends on the specific timing of kernel overlap. Our analysis reveals which kernel combinations create worst-case scenarios.

### Finding 4: Current Abstractions Hide Critical Information
Framework developers cannot observe these issues without hardware-level profiling, preventing software-only solutions.

---

## Impact & Significance

### For Framework Developers
- Awareness of hidden performance costs in scheduling decisions
- Insights for smarter kernel placement and execution strategies
- Motivation for better cross-layer visibility

### For Hardware Architects
- Understanding of real-world contention patterns in distributed training
- Requirements for next-generation GPU architectures
- Opportunities for hardware support for better resource isolation

### For ML Practitioners
- Better understanding of performance trade-offs in distributed training
- Guidance for configuration decisions
- Awareness of scaling limitations

---

## Tools & Technologies

**Frameworks & Libraries**:
- Megatron-LM (NVIDIA's distributed training framework)
- PyTorch (deep learning framework)
- NCCL (NVIDIA Collective Communications Library)

**Profiling & Analysis**:
- NVIDIA Nsight Compute
- NVIDIA Nsight Systems  
- PyTorch Profiler
- Custom profiling instrumentation

**Hardware Platform**:
- NVIDIA A100 GPUs (Ampere Architecture)
- NVIDIA H100 GPUs (Hopper Architecture)
- NVLink high-bandwidth interconnect

---

## Presentation

**Venue**: IEEE International Symposium on Performance Analysis of Systems and Software (ISPASS 2025)  
**Format**: Poster Presentation  
**Presenter**: Jihwan Oh (Second Author)

The poster presentation generated significant interest from:
- Researchers working on distributed training optimization
- GPU architecture designers
- Framework developers from industry and academia

Valuable discussions during the conference have informed our ongoing follow-up research.

---

## Follow-up Research

This work has spawned active follow-up research directions:

### 1. **TMA-Based Optimization** (Ongoing)
Building on these findings, I am leading research to develop practical solutions:
- Leveraging NVIDIA Hopper's Tensor Memory Accelerator (TMA)
- Using idle shared memory as intermediate buffers
- Reducing data path to decrease SM requirements
- Achieving measurable performance improvements

### 2. **NCCL Protocol Enhancement** (In Progress)
Integrating our optimizations into NCCL as a new collective communication protocol to benefit the broader community.

### 3. **Generalization to Other Workloads**
Investigating whether similar patterns appear in other distributed computing scenarios beyond deep learning training.

---

## Related Publications

*This is my first publication. Future work building on these findings is in progress.*

---

## Code & Data

*Code and profiling data availability to be determined based on collaboration agreements.*

---

## Collaborators

This work was conducted in collaboration with researchers at:
- Georgia Institute of Technology (Advisor: Prof. Divya Mahajan)
- KAIST (Advisor: Prof. Jongse Park)

---

## Lessons Learned

This project taught me invaluable lessons about computer architecture research:

1. **Cross-layer thinking is essential**: Problems at one layer often have root causes at another
2. **Abstractions are powerful but can hide problems**: Need tools and methodologies that work across layers
3. **Real systems are complex**: Production frameworks reveal issues not visible in simplified benchmarks
4. **Persistent profiling pays off**: Deep investigation reveals insights that surface-level analysis misses
5. **Collaboration enhances research**: Working across institutions brought diverse perspectives

These lessons continue to guide my ongoing research and shape my vision for my Ph.D. work.

---

*For more information or to discuss this work, please contact me at [jihwanoh1@gatech.edu](mailto:jihwanoh1@gatech.edu) or [dhdudrby@kaist.ac.kr](mailto:dhdudrby@kaist.ac.kr).*

