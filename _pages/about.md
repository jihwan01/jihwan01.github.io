---
permalink: /
title: "Jihwan Oh"
excerpt: "Computer Architecture, Systems for ML, and Hardware-Software Co-Design"
author_profile: false
hide_title: true
redirect_from:
  - /about/
  - /about.html
---

<style>
  .jo-profile {
    --jo-ink: var(--global-text-color);
    --jo-muted: #625a52;
    --jo-line: var(--global-border-color);
    --jo-rule: #eee8e1;
    --jo-card: var(--global-bg-color);
    --jo-soft: #faf7f3;
    --jo-avatar-bg: #f7f2ed;
    --jo-chip-bg: #f3eee8;
    --jo-chip-text: #4d4037;
    --jo-authors: #3b352f;
    --jo-button-bg: var(--global-bg-color);
    --jo-primary-text: #fff;
    --jo-cardinal: #8c1515;
    --jo-green: #1f6f5f;
    --jo-gold: #8f641f;
    --jo-blue: #2f5d8c;
    --jo-plum: #7a4d8f;
    --jo-rust: #9a4d1f;
    color: var(--jo-ink);
  }

  html[data-theme="dark"] .jo-profile {
    --jo-muted: #f3f3f3;
    --jo-line: rgba(255, 255, 255, 0.32);
    --jo-rule: rgba(255, 255, 255, 0.18);
    --jo-card: #505050;
    --jo-soft: #505050;
    --jo-avatar-bg: #555;
    --jo-chip-bg: #5f5751;
    --jo-chip-text: #fff;
    --jo-authors: #fff;
    --jo-button-bg: #505050;
    --jo-cardinal: #ffb3b3;
    --jo-green: #9de0d4;
    --jo-gold: #f0c37a;
    --jo-blue: #a8cbf0;
    --jo-plum: #d7b6ef;
    --jo-rust: #f2b78c;
  }

  .jo-profile a {
    color: var(--jo-cardinal);
    font-weight: 650;
    text-decoration-thickness: 1px;
    text-underline-offset: 3px;
  }

  .jo-profile a:hover {
    color: var(--section-accent, var(--jo-cardinal));
  }

  .jo-hero {
    padding: 28px 0 32px;
    border-bottom: 1px solid var(--jo-line);
  }

  .jo-hero-layout {
    max-width: 920px;
  }

  .jo-identity {
    display: flex;
    align-items: center;
    gap: 20px;
    margin-bottom: 22px;
  }

  .jo-portrait {
    flex: 0 0 auto;
    position: relative;
    width: 112px;
    height: 112px;
    border-radius: 50%;
    background:
      radial-gradient(circle at 50% 50%, var(--jo-card) 0 67%, transparent 68%),
      conic-gradient(from 150deg, var(--jo-cardinal), var(--jo-gold), var(--jo-green), var(--jo-cardinal));
  }

  .jo-portrait::after {
    content: "";
    position: absolute;
    inset: 7px;
    border-radius: 50%;
    border: 1px solid var(--jo-line);
    pointer-events: none;
  }

  .jo-photo {
    position: absolute;
    inset: 9px;
    display: block;
    width: calc(100% - 18px);
    height: calc(100% - 18px);
    border-radius: 50%;
    object-fit: cover;
    object-position: center 27%;
    border: 1px solid var(--jo-line);
    background: var(--jo-avatar-bg);
    box-shadow: 0 14px 34px rgba(0, 0, 0, 0.16);
  }

  html[data-theme="dark"] .jo-photo {
    box-shadow: none;
  }

  .jo-title-block {
    min-width: 0;
  }

  .jo-hero h1 {
    margin: 0;
    font-size: 3.2rem;
    line-height: 0.95;
    letter-spacing: 0;
  }

  .jo-affiliation {
    margin: 10px 0 0;
    color: var(--jo-muted);
    font-size: 1rem;
    font-weight: 650;
    line-height: 1.45;
  }

  .jo-lead {
    max-width: 900px;
    margin: 0;
    color: var(--jo-ink);
    font-size: 1.55rem;
    font-weight: 700;
    line-height: 1.22;
  }

  .jo-copy {
    max-width: 860px;
    margin: 18px 0 0;
    color: var(--jo-muted);
    font-size: 1rem;
    line-height: 1.75;
  }

  .jo-actions {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 22px;
  }

  .jo-button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 40px;
    padding: 8px 14px;
    border: 1px solid var(--jo-line);
    border-radius: 6px;
    background: var(--jo-button-bg);
    color: var(--jo-ink) !important;
    font-size: 0.86rem;
    font-weight: 700;
    text-decoration: none !important;
  }

  .jo-button.primary {
    border-color: var(--jo-cardinal);
    background: var(--jo-cardinal);
    color: var(--jo-primary-text) !important;
  }

  .jo-section {
    --section-accent: var(--jo-cardinal);
    --section-chip-bg: var(--jo-chip-bg);
    padding: 28px 0;
    border-bottom: 1px solid var(--jo-line);
  }

  .jo-section a {
    color: var(--section-accent);
  }

  .jo-section h2 {
    margin: 0 0 18px;
    color: var(--section-accent);
    font-size: 1.55rem;
    line-height: 1.15;
  }

  .jo-section h2::before {
    content: "";
    display: inline-block;
    width: 10px;
    height: 10px;
    margin-right: 10px;
    border-radius: 50%;
    background: var(--section-accent);
    vertical-align: 0.08em;
  }

  #news {
    --section-accent: var(--jo-cardinal);
    --section-chip-bg: color-mix(in srgb, var(--jo-cardinal) 12%, var(--jo-chip-bg));
  }

  #research {
    --section-accent: var(--jo-green);
    --section-chip-bg: color-mix(in srgb, var(--jo-green) 14%, var(--jo-chip-bg));
  }

  #publications {
    --section-accent: var(--jo-blue);
    --section-chip-bg: color-mix(in srgb, var(--jo-blue) 14%, var(--jo-chip-bg));
  }

  #experience {
    --section-accent: var(--jo-rust);
    --section-chip-bg: color-mix(in srgb, var(--jo-rust) 14%, var(--jo-chip-bg));
  }

  #education {
    --section-accent: var(--jo-plum);
    --section-chip-bg: color-mix(in srgb, var(--jo-plum) 14%, var(--jo-chip-bg));
  }

  #honors,
  #contact {
    --section-accent: var(--jo-gold);
    --section-chip-bg: color-mix(in srgb, var(--jo-gold) 14%, var(--jo-chip-bg));
  }

  .jo-section-intro {
    max-width: 820px;
    margin: -6px 0 20px;
    color: var(--jo-muted);
    line-height: 1.7;
  }

  .jo-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 14px;
  }

  .jo-card {
    padding: 18px;
    border: 1px solid var(--jo-line);
    border-radius: 8px;
    background: var(--jo-card);
  }

  .jo-card h3 {
    margin: 0 0 10px;
    font-size: 1.02rem;
    line-height: 1.3;
  }

  .jo-card p {
    margin: 0;
    color: var(--jo-muted);
    line-height: 1.62;
  }

  .jo-education {
    display: grid;
    gap: 14px;
  }

  .jo-education-item {
    display: grid;
    grid-template-columns: 120px minmax(0, 1fr);
    gap: 18px;
    padding: 18px;
    border: 1px solid var(--jo-line);
    border-radius: 8px;
    background: var(--jo-card);
  }

  .jo-education-item h3 {
    margin: 0 0 4px;
    font-size: 1.08rem;
    line-height: 1.3;
  }

  .jo-degree {
    margin: 0;
    color: var(--jo-ink);
    font-weight: 700;
    line-height: 1.45;
  }

  .jo-edu-meta {
    margin: 6px 0 0;
    color: var(--jo-muted);
    line-height: 1.55;
  }

  .jo-edu-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 7px;
    margin-top: 12px;
  }

  .jo-edu-tags span {
    display: inline-flex;
    align-items: center;
    min-height: 26px;
    padding: 4px 8px;
    border-radius: 999px;
    background: var(--section-chip-bg);
    color: var(--jo-chip-text);
    font-size: 0.75rem;
    font-weight: 700;
  }

  .jo-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 7px;
    margin-top: 14px;
  }

  .jo-tags span,
  .jo-pub-meta span {
    display: inline-flex;
    align-items: center;
    min-height: 26px;
    padding: 4px 8px;
    border-radius: 999px;
    background: var(--section-chip-bg);
    color: var(--jo-chip-text);
    font-size: 0.75rem;
    font-weight: 700;
  }

  .jo-news,
  .jo-list {
    display: grid;
    gap: 12px;
  }

  .jo-news-item,
  .jo-timeline-item {
    display: grid;
    grid-template-columns: 120px minmax(0, 1fr);
    gap: 18px;
    padding-bottom: 12px;
    border-bottom: 1px solid var(--jo-rule);
  }

  .jo-date {
    color: var(--jo-gold);
    font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, monospace;
    font-size: 0.78rem;
    font-weight: 700;
  }

  .jo-news-item p,
  .jo-timeline-item p,
  .jo-timeline-item ul {
    margin: 0;
    color: var(--jo-muted);
    line-height: 1.62;
  }

  .jo-publication {
    padding: 18px 0;
    border-bottom: 1px solid var(--jo-rule);
  }

  .jo-pub-meta {
    display: flex;
    flex-wrap: wrap;
    gap: 7px;
    margin-bottom: 10px;
  }

  .jo-publication h3 {
    margin: 0;
    font-size: 1.08rem;
    line-height: 1.35;
  }

  .jo-authors {
    margin: 8px 0 0 !important;
    color: var(--jo-authors) !important;
    font-weight: 600;
  }

  .jo-role {
    color: var(--jo-green) !important;
    font-weight: 700;
  }

  .jo-timeline-item ul {
    margin-top: 8px;
    padding-left: 18px;
  }

  .jo-contact {
    padding: 20px;
    border: 1px solid var(--jo-line);
    border-radius: 8px;
    background: var(--jo-soft);
  }

  .jo-contact p {
    margin: 0 0 10px;
    color: var(--jo-muted);
    line-height: 1.65;
  }

  @media (max-width: 760px) {
    .jo-hero h1 {
      font-size: 2.4rem;
    }

    .jo-identity {
      align-items: flex-start;
      gap: 14px;
      margin-bottom: 18px;
    }

    .jo-portrait {
      width: 78px;
      height: 78px;
    }

    .jo-lead {
      font-size: 1.25rem;
    }

    .jo-grid,
    .jo-education-item,
    .jo-news-item,
    .jo-timeline-item {
      grid-template-columns: 1fr;
    }

    .jo-news-item,
    .jo-timeline-item {
      gap: 4px;
    }
  }
</style>

<div class="jo-profile">
  <section class="jo-hero">
    <div class="jo-hero-layout">
      <div class="jo-identity">
        <div class="jo-portrait">
          <img class="jo-photo" src="/images/jihwan_profile.jpeg" alt="Jihwan Oh">
        </div>
        <div class="jo-title-block">
          <h1>Jihwan Oh</h1>
          <p class="jo-affiliation">Ph.D. Student in Electrical Engineering, Stanford University</p>
        </div>
      </div>
      <p class="jo-lead">
        I work on cross-layer optimization and hardware-software co-design for energy-efficient, high-performance computing systems.
      </p>
      <p class="jo-copy">
        I am starting my Ph.D. in <a href="https://ee.stanford.edu/">Stanford EE</a> with <a href="https://tambelab.stanford.edu/">Prof. Thierry Tambe</a>. Previously, I worked with <a href="https://www.divyamahajan.com/">Prof. Divya Mahajan</a> at <a href="https://www.gatech.edu/">Georgia Tech</a> and completed my B.S. at <a href="https://kaist.ac.kr/">KAIST</a>.
      </p>
      <div class="jo-actions">
        <a class="jo-button primary" href="/files/CV_JihwanOh.pdf">CV</a>
        <a class="jo-button" href="mailto:jihwanoh@stanford.edu">Email</a>
        <a class="jo-button" href="https://github.com/jihwan01">GitHub</a>
        <a class="jo-button" href="https://scholar.google.com/citations?user=Ajs3-gwAAAAJ&hl=ko&oi=sra">Google Scholar</a>
      </div>
    </div>
  </section>

  <section class="jo-section" id="news">
    <h2>News</h2>
    <div class="jo-news">
      <div class="jo-news-item">
        <span class="jo-date">Sep 2026</span>
        <p>Starting the Ph.D. program in Electrical Engineering at Stanford University and joining Prof. Thierry Tambe Lab.</p>
      </div>
      <div class="jo-news-item">
        <span class="jo-date">Jul 2026</span>
        <p>First-author paper accepted to IEEE International Symposium on Workload Characterization (IISWC) 2026.</p>
      </div>
      <div class="jo-news-item">
        <span class="jo-date">Jun 2025</span>
        <p>Selected as a full travel grant recipient for ISCA 2025 and the uArch Workshop in Tokyo.</p>
      </div>
      <div class="jo-news-item">
        <span class="jo-date">May 2025</span>
        <p>Presented work on compute-communication overlap at ISPASS 2025 in Ghent.</p>
      </div>
    </div>
  </section>

  <section class="jo-section" id="research">
    <h2>Research Interests</h2>
    <p class="jo-section-intro">
      My research asks how hardware, runtime systems, communication protocols, and ML workloads can be designed together instead of optimized in isolation.
    </p>
    <div class="jo-grid">
      <div class="jo-card">
        <h3>Cross-Layer Systems</h3>
        <p>Profiling and redesigning the interaction between GPU kernels, communication libraries, runtimes, and hardware resources.</p>
        <div class="jo-tags"><span>NCCL</span><span>CUDA</span><span>Nsight</span></div>
      </div>
      <div class="jo-card">
        <h3>Hardware-Software Co-Design</h3>
        <p>Building mechanisms that improve performance and energy efficiency across the full computing stack.</p>
        <div class="jo-tags"><span>GPU systems</span><span>Memory systems</span><span>Pipelining</span></div>
      </div>
      <div class="jo-card">
        <h3>Specialized Accelerators</h3>
        <p>Studying accelerator architectures for data-intensive ML workloads, including PIM and domain-specific execution.</p>
        <div class="jo-tags"><span>PIM</span><span>LLM inference</span><span>Architecture</span></div>
      </div>
    </div>
  </section>

  <section class="jo-section" id="publications">
    <h2>Selected Publications</h2>
    <article class="jo-publication">
      <div class="jo-pub-meta"><span>IISWC 2026</span><span>Conference</span></div>
      <h3>Regular-Compute-Communication Overlap Is Not Free: A Cross-Layer Characterization in GPU LLM Workloads</h3>
      <p class="jo-authors"><strong>Jihwan Oh</strong>, Seokjin Go, Junkyum Kim, Jongse Park, Divya Mahajan</p>
      <p class="jo-copy">A cross-layer study of compute-communication overlap overheads in GPU LLM workloads, exposing hardware-level costs that can be hidden at the software layer.</p>
    </article>
    <article class="jo-publication">
      <div class="jo-pub-meta"><span>ISPASS 2025</span><span>Poster</span></div>
      <h3>Characterizing Compute-Communication Overlap in GPU-Accelerated Distributed Deep Learning: Performance and Power Implications</h3>
      <p class="jo-authors">Seonho Lee, <strong>Jihwan Oh</strong>, Junkyum Kim, Seokjin Go, Jongse Park, Divya Mahajan</p>
      <p class="jo-copy">Shows that aggressively maximizing overlap in distributed deep learning can degrade both execution time and power efficiency across parallelism configurations.</p>
      <p class="jo-copy"><a href="https://arxiv.org/abs/2507.03114">arXiv:2507.03114</a></p>
    </article>
  </section>

  <section class="jo-section" id="experience">
    <h2>Experience</h2>
    <div class="jo-list">
      <div class="jo-timeline-item">
        <span class="jo-date">Jan 2025 - Aug 2026</span>
        <div>
          <h3><a href="https://www.divyamahajan.com/">Systems Infrastructure and Architecture Research Lab</a>, <a href="https://www.gatech.edu/">Georgia Tech</a></h3>
          <p class="jo-role">Researcher, advised by <a href="https://www.divyamahajan.com/">Prof. Divya Mahajan</a></p>
          <ul>
            <li>Characterized compute-communication overlap in large-scale distributed LLM training.</li>
            <li>Led profiling work to identify hardware-level sources of overlap overhead.</li>
            <li>Designed an NCCL cross-layer communication protocol using shared memory as a TMA-driven staging buffer.</li>
          </ul>
        </div>
      </div>
      <div class="jo-timeline-item">
        <span class="jo-date">Sep 2024 - Dec 2024</span>
        <div>
          <h3>Computer Architecture and Systems Lab, <a href="https://kaist.ac.kr/">KAIST</a></h3>
          <p class="jo-role">Undergraduate Researcher, advised by <a href="https://jongse-park.github.io/">Prof. Jongse Park</a></p>
          <ul>
            <li>Analyzed LLM inference on NeuPIMs and studied NPU-PIM load imbalance.</li>
            <li>Explored redistribution strategies and quantization techniques for PIM architectures.</li>
          </ul>
        </div>
      </div>
      <div class="jo-timeline-item">
        <span class="jo-date">Aug 2021 - May 2023</span>
        <div>
          <h3>Republic of Korea Air Force</h3>
          <p class="jo-role">Software Developer</p>
          <ul>
            <li>Developed a VR flight-training system with Unreal Engine 4 and C++.</li>
            <li>Presented the simulator as an Air Force representative at a national information and communication development conference.</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <section class="jo-section" id="education">
    <h2>Education</h2>
    <div class="jo-education">
      <div class="jo-education-item">
        <span class="jo-date">Sep 2026 -</span>
        <div>
          <h3>Stanford University</h3>
          <p class="jo-degree">Ph.D. in Electrical Engineering</p>
          <p class="jo-edu-meta">Advisor: Prof. Thierry Tambe Lab</p>
          <div class="jo-edu-tags"><span>Ph.D.</span><span>Electrical Engineering</span><span>Stanford, CA</span></div>
        </div>
      </div>
      <div class="jo-education-item">
        <span class="jo-date">Feb 2019 - Feb 2026</span>
        <div>
          <h3>KAIST</h3>
          <p class="jo-degree">B.S. in Electrical Engineering</p>
          <p class="jo-edu-meta">Double major in School of Computing. GPA 4.07/4.3.</p>
          <div class="jo-edu-tags"><span>Summa Cum Laude</span><span>Dean's List</span><span>Daejeon, Korea</span></div>
        </div>
      </div>
      <div class="jo-education-item">
        <span class="jo-date">Jan 2025 - Jul 2025</span>
        <div>
          <h3>Georgia Institute of Technology</h3>
          <p class="jo-degree">Exchange Program, School of Electrical and Computer Engineering</p>
          <p class="jo-edu-meta">GPA 4.0/4.0.</p>
          <div class="jo-edu-tags"><span>Exchange Student</span><span>ECE</span><span>Atlanta, GA</span></div>
        </div>
      </div>
    </div>
  </section>

  <section class="jo-section" id="honors">
    <h2>Honors & Awards</h2>
    <ul>
      <li>Next-Generation Engineer Award: Highest Distinction, IPESK, 2025</li>
      <li>uArch Mentoring Workshop Full Travel Grant, uArch @ ISCA 2025</li>
      <li>Student Travel Grant, IEEE ISPASS 2025</li>
      <li>Korea-U.S. Student Exchange Program Scholarship, KIAT, 2024</li>
      <li>National Science and Technology Scholarship, Korea Government, 2021 - 2024</li>
    </ul>
  </section>

  <section class="jo-section" id="contact">
    <h2>Contact</h2>
    <div class="jo-contact">
      <p>Open to research conversations around efficient AI systems, architecture, and internship opportunities.</p>
      <p><a href="mailto:jihwanoh@stanford.edu">jihwanoh@stanford.edu</a> | <a href="/files/CV_JihwanOh.pdf">CV</a> | <a href="https://scholar.google.com/citations?user=Ajs3-gwAAAAJ&hl=ko&oi=sra">Google Scholar</a> | <a href="https://github.com/jihwan01">GitHub</a></p>
    </div>
  </section>
</div>
