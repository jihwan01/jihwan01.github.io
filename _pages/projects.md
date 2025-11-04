---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

{% include base_path %}

<div style="position: fixed; top: 80px; right: 20px; width: 200px; padding: 15px; background: #f8f9fa; border-radius: 8px; box-shadow: 0 2px 4px rgba(0,0,0,0.1); z-index: 10;">
  <h4 style="margin-top: 0; font-size: 1em; color: #333;">📋 Sections</h4>
  <ul style="list-style: none; padding-left: 0; margin: 0; font-size: 0.9em;">
    <li style="margin-bottom: 8px;"><a href="#research-projects" style="color: #0366d6; text-decoration: none;">Research Projects</a></li>
    <li style="margin-bottom: 8px;"><a href="#engineering-projects" style="color: #0366d6; text-decoration: none;">Engineering Projects</a></li>
    <li style="margin-bottom: 8px;"><a href="#leadership--extracurricular" style="color: #0366d6; text-decoration: none;">Leadership & Extracurricular</a></li>
  </ul>
</div>

<div style="padding: 15px 20px; background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); border-radius: 8px; margin-bottom: 30px;">
  <h2 id="research-projects" style="color: white; margin: 0; font-size: 1.8em;">🔬 Research Projects</h2>
</div>

<div style="background: #ffffff; border: 1px solid #e1e4e8; border-radius: 10px; padding: 25px; margin-bottom: 25px; box-shadow: 0 2px 8px rgba(0,0,0,0.08);">

<h3 style="margin-top: 0; color: #24292e;"><strong>GPU-Accelerated Distributed Deep Learning Optimization</strong> (Ongoing)</h3>
<p style="color: #666; font-style: italic; margin: 5px 0;">Systems Infrastructure and Architecture Research Lab, Georgia Tech</p>
<p style="color: #0366d6; font-weight: 500; margin: 5px 0;">Advisor: Prof. Divya Mahajan</p>

<p style="margin-top: 15px; line-height: 1.6;">Leading follow-up research to develop solutions for mitigating overhead occurred in concurrent execution between computation and communication in distributed LLM training. Conducted kernel-level profiling to identify root causes of performance degradation, revealing that hardware resource contention, obscured by software abstractions, causes individual kernels to execute slower despite end-to-end latency improvements from pipelining.</p>

<p style="margin-top: 12px; line-height: 1.6;">Built custom micro-benchmarks to analyze hardware resource utilization patterns. Developing novel optimization techniques leveraging modern GPU architecture features to improve communication efficiency, with initial results showing promising performance improvements.</p>

</div>

<div style="background: #ffffff; border: 1px solid #e1e4e8; border-radius: 10px; padding: 25px; margin-bottom: 25px; box-shadow: 0 2px 8px rgba(0,0,0,0.08);">

<h3 style="margin-top: 0; color: #24292e;"><strong>Characterizing Performance Impact of Compute-Communication Overlap in Distributed Training</strong></h3>
<p style="color: #666; font-style: italic; margin: 5px 0;">Systems Infrastructure and Architecture Research Lab, Georgia Tech</p>
<p style="color: #0366d6; font-weight: 500; margin: 5px 0;">Advisor: Prof. Divya Mahajan</p>

<p style="margin-top: 15px; line-height: 1.6;">Characterized performance overhead when compute and communication operations execute concurrently for latency hiding in distributed LLM training. Analyzed how overlap timing affects end-to-end latency and energy consumption across different parallelism strategies and model sizes.</p>

<p style="margin-top: 12px; line-height: 1.6;">Conducted comprehensive experiments using Megatron-LM framework across various configurations, uncovering critical insights about the trade-offs between concurrent execution and resource contention in large-scale distributed training systems.</p>

<p style="margin-top: 15px;"><strong>Publication:</strong> <a href="https://arxiv.org/abs/2507.03114" target="_blank">IEEE ISPASS 2025</a> (2nd author, poster presentation)</p>

</div>

<div style="background: #ffffff; border: 1px solid #e1e4e8; border-radius: 10px; padding: 25px; margin-bottom: 25px; box-shadow: 0 2px 8px rgba(0,0,0,0.08);">

<h3 style="margin-top: 0; color: #24292e;"><strong>NPU-PIM Heterogeneous System Optimization, Domain specific optimization</strong></h3>
<p style="color: #666; font-style: italic; margin: 5px 0;">Computer Architecture and Systems Lab, KAIST</p>
<p style="color: #0366d6; font-weight: 500; margin: 5px 0;">Advisor: Prof. Jongse Park</p>

<p style="margin-top: 15px; line-height: 1.6;">Developed workload balancing strategies for heterogeneous NPU-PIM systems based on <em>NeuPIMs</em> (ASPLOS 2024). </p>

</div>

<div style="background: #ffffff; border: 1px solid #e1e4e8; border-radius: 10px; padding: 25px; margin-bottom: 25px; box-shadow: 0 2px 8px rgba(0,0,0,0.08);">

<h3 style="margin-top: 0; color: #24292e;"><strong>Mobile Robotics Path Planning</strong></h3>
<p style="color: #666; font-style: italic; margin: 5px 0;">Urban Robotics Lab, KAIST</p>
<p style="color: #0366d6; font-weight: 500; margin: 5px 0;">Advisor: Prof. Hyun Myung</p>

<p style="margin-top: 15px; line-height: 1.6;">Implemented SLAM algorithms and developed ROS-based autonomous navigation systems for mobile robotics applications.</p>

</div>

<div style="padding: 15px 20px; background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%); border-radius: 8px; margin: 40px 0 30px 0;">
  <h2 id="engineering-projects" style="color: white; margin: 0; font-size: 1.8em;">⚙️ Engineering Projects</h2>
</div>

<div style="background: #ffffff; border: 1px solid #e1e4e8; border-radius: 10px; padding: 25px; margin-bottom: 25px; box-shadow: 0 2px 8px rgba(0,0,0,0.08);">

<h3 style="margin-top: 0; color: #24292e;"><strong>VR Flight Simulator</strong></h3>
<p style="color: #666; font-style: italic; margin: 5px 0;">Unreal Engine 4 & C++</p>

<p style="margin-top: 15px; line-height: 1.6;">Developed an immersive VR flight simulator using Unreal Engine 4 and C++ for pilot training applications. The system features realistic cockpit controls, dynamic weather conditions, and VR headset integration to provide trainees with hands-on flight experience in a safe, controlled environment.</p>

<p style="font-weight: 600; margin: 15px 0 10px 0; color: #333;">Project Demo</p>
<div style="max-width: 700px; margin: 0;">
  <div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden;">
    <iframe style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border-radius: 8px;" src="https://www.youtube.com/embed/0U3ZDx9tsZg" title="VR Flight Simulator Demo" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
  </div>
</div>

</div>

<div style="background: #ffffff; border: 1px solid #e1e4e8; border-radius: 10px; padding: 25px; margin-bottom: 25px; box-shadow: 0 2px 8px rgba(0,0,0,0.08);">

<h3 style="margin-top: 0; color: #24292e;"><strong>Customized LLM for AI Education</strong></h3>
<p style="color: #666; font-style: italic; margin: 5px 0;">Georgia Tech - AI First Course Project</p>

<p style="margin-top: 15px; line-height: 1.6;">Domain-specific LLM fine-tuned for AI education, achieving 82% BERTScore improvement over the provided baseline model.</p>

<div style="margin-top: 15px; max-width: 600px;">
  <a href="/files/AIFIRST_FINAL_PROJECT_POSTER_JIHWANOH.pdf" target="_blank">
    <img src="/files/AIFIRST_POSTER.png" alt="AI First Project Poster" style="width: 100%; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.1); cursor: pointer;">
  </a>
</div>

<p style="margin-top: 15px;">🔗 <a href="https://github.com/jihwan01/AIFirst_Customized_LLM" target="_blank">GitHub Repository</a></p>

</div>

<div style="background: #ffffff; border: 1px solid #e1e4e8; border-radius: 10px; padding: 25px; margin-bottom: 25px; box-shadow: 0 2px 8px rgba(0,0,0,0.08);">

<h3 style="margin-top: 0; color: #24292e;"><strong>BARD: Autonomous Desk Cleaning Robot</strong></h3>
<p style="color: #666; font-style: italic; margin: 5px 0;">Georgia Tech - Embedded Systems Design</p>

<p style="margin-top: 15px; line-height: 1.6;">Arduino-based autonomous robot with cliff detection, obstacle avoidance, and 180-degree environmental scanning.</p>

<div style="margin-top: 15px; max-width: 600px;">
  <div style="display: grid; grid-template-columns: repeat(4, 1fr); gap: 6px;">
    <img src="/files/bard_gifs/vacuum.gif" alt="BARD Vacuum" style="width: 100%; height: 120px; object-fit: cover; border-radius: 6px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
    <img src="/files/bard_gifs/edge_rot.gif" alt="BARD Edge Detection" style="width: 100%; height: 120px; object-fit: cover; border-radius: 6px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
    <img src="/files/bard_gifs/forward.gif" alt="BARD Forward Movement" style="width: 100%; height: 120px; object-fit: cover; border-radius: 6px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
    <img src="/files/bard_gifs/get_around_distance.gif" alt="BARD Distance Scanning" style="width: 100%; height: 120px; object-fit: cover; border-radius: 6px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
  </div>
</div>

<p style="margin-top: 15px;">🔗 <a href="https://github.com/jihwan01/desk_cleaning_robot" target="_blank">GitHub Repository</a></p>

</div>

<div style="background: #ffffff; border: 1px solid #e1e4e8; border-radius: 10px; padding: 25px; margin-bottom: 25px; box-shadow: 0 2px 8px rgba(0,0,0,0.08);">

<h3 style="margin-top: 0; color: #24292e;"><strong>Jip-Sa - Rental Fraud Prevention Platform</strong></h3>
<p style="color: #666; font-style: italic; margin: 5px 0;">KAIST Immersion Camp</p>

<p style="margin-top: 15px; line-height: 1.6;">Web platform leveraging Korea's Public Data Portal to analyze 170,000+ real estate transactions and assess rental fraud risk levels for individual officetel units.</p>

<div style="margin-top: 15px; max-width: 700px;">
  <div style="display: grid; grid-template-columns: 1fr; gap: 10px;">
    <img src="https://github.com/Jip-Sa/Jip-Sa-Back/assets/43375122/5bb951f9-a6fd-4ed7-ac34-18e44efee6a9" alt="Jip-Sa Map View" style="width: 100%; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
  </div>
</div>

<p style="margin-top: 15px;">🔗 <a href="https://github.com/Jip-Sa" target="_blank">GitHub Repository</a></p>

</div>

<div style="background: #ffffff; border: 1px solid #e1e4e8; border-radius: 10px; padding: 25px; margin-bottom: 25px; box-shadow: 0 2px 8px rgba(0,0,0,0.08);">

<h3 style="margin-top: 0; color: #24292e;"><strong>Imp (하루, 셈) - Daily Reflection Journal App</strong></h3>
<p style="color: #666; font-style: italic; margin: 5px 0;">KAIST Immersion Camp</p>

<p style="margin-top: 15px; line-height: 1.6;">React Native app for daily reflection with customizable question templates and social features.</p>

<div style="margin-top: 15px; max-width: 600px;">
  <div style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 8px;">
    <img src="https://github.com/ImpDay/Imp_Front/assets/61741090/64d6e6f8-e6bc-43b3-9328-0f38c86374d4" alt="Imp Login" style="width: 100%; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
    <img src="https://github.com/ImpDay/Imp_Front/assets/61741090/c0184d5b-86f9-413c-9770-dbe7a28ebcf5" alt="Imp Home" style="width: 100%; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
    <img src="https://github.com/ImpDay/Imp_Front/assets/61741090/e6a39c81-9113-4029-8b45-a2d5d4ad702c" alt="Imp Friends" style="width: 100%; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
  </div>
</div>

<p style="margin-top: 15px;">🔗 <a href="https://github.com/ImpDay/Imp_Front" target="_blank">GitHub Repository</a></p>

</div>

<div style="padding: 15px 20px; background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%); border-radius: 8px; margin: 40px 0 30px 0;">
  <h2 id="leadership--extracurricular" style="color: white; margin: 0; font-size: 1.8em;">🌟 Leadership & Extracurricular</h2>
</div>

<div style="background: #ffffff; border: 1px solid #e1e4e8; border-radius: 10px; padding: 25px; margin-bottom: 25px; box-shadow: 0 2px 8px rgba(0,0,0,0.08);">

<h3 style="margin-top: 0; color: #24292e;"><strong>ICISTS, Public Relations Head</strong></h3>
<p style="color: #666; font-style: italic; margin: 5px 0;">Student-led Startup Conference</p>

<p style="margin-top: 15px; line-height: 1.6;">Led PR campaigns for GRAFFITI conference, growing attendance to 150+ participants.</p>

<p style="font-weight: 600; margin: 15px 0 10px 0; color: #333;">Promotional Videos</p>
<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 15px; max-width: 700px;">
  <div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden;">
    <iframe src="https://www.youtube.com/embed/nYK91YwynRc" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border-radius: 8px;"></iframe>
  </div>
  <div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden;">
    <iframe src="https://www.youtube.com/embed/Wmzp6ea4DW4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border-radius: 8px;"></iframe>
  </div>
</div>

</div>

<div style="background: #ffffff; border: 1px solid #e1e4e8; border-radius: 10px; padding: 25px; margin-bottom: 25px; box-shadow: 0 2px 8px rgba(0,0,0,0.08);">

<h3 style="margin-top: 0; color: #24292e;"><strong>KAIST Buddy Program</strong></h3>
<p style="color: #666; font-style: italic; margin: 5px 0;">International Student Support</p>

<p style="margin-top: 15px; line-height: 1.6;">Mentored international exchange students on academic and cultural adaptation.</p>

</div>

<div style="background: #ffffff; border: 1px solid #e1e4e8; border-radius: 10px; padding: 25px; margin-bottom: 25px; box-shadow: 0 2px 8px rgba(0,0,0,0.08);">

<h3 style="margin-top: 0; color: #24292e;"><strong>Summer Mentoring Camp</strong></h3>
<p style="color: #666; font-style: italic; margin: 5px 0;">Rural Education Initiative</p>

<p style="margin-top: 15px; line-height: 1.6;">Delivered STEM education and career mentoring to rural middle school students.</p>

</div>

---

<div style="text-align: center; margin-top: 30px; padding: 15px; background-color: #f0f8ff; border-radius: 8px;">
  <p><strong>Interested in collaboration?</strong></p>
  <p>📧 <a href="mailto:jihwanoh1@gatech.edu">jihwanoh1@gatech.edu</a> | <a href="mailto:dhdudrby@kaist.ac.kr">dhdudrby@kaist.ac.kr</a></p>
</div>
