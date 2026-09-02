+++
title = "Nathan's Autonomous Materials Research Portfolio"
type = "portfolio"
layout = "single"
draft = false
description = "Research portfolio: agentic AI for scientific instrumentation, autonomous laboratories, and materials science."

# Keep this page off the sitemap, the homepage, and any list page —
# reachable only by whoever has the direct link.
[build]
  list = "never"
  render = "always"

[params]
  robots = "noindex, nofollow"
+++
I've spent my career at the intersection of materials experimentation
and the algorithms that drive those experiments. This page is the technical,
work-focused version of me: what I've built, what I've run, and what I've 
learned about the gap between a model that can reason and a model that can 
safely turn a knob.

Lately I've been building AI agents that drive scientific instruments — 
the kind with beam currents, vacuum interlocks, and a five-figure repair 
bill if you get it wrong. 

## What I actually do

### Agentic control of complex scientific instruments

At Zeiss I lead development of LLM-controlled microscopy systems for X-ray
and electron microscopes — agents that plan, call tools, generate code,
verify their own outputs, and operate real hardware across long, multi-step
characterization workflows. That means typed instrument APIs (MCP/FastMCP),
structured function calling instead of hopeful text parsing, working memory
for tasks that span dozens of steps, multi-agent orchestration, and telemetry
detailed enough to explain a failure after the fact rather than just observe
one. I've also built the benchmark suites and evaluation harnesses that ask
the less glamorous question: does any of this actually generalize, or did it
just memorize the demo?

### Materials theory meets active experimentation

Before building autonomous microscopes, I was on the other side of the
closed loop: using Bayesian experimental design and active-learning models
to decide what to synthesize next, and pairing DFT with high-throughput
synchrotron beamlines to make combinatorial materials discovery something
you could actually finish in a PhD. At Stanford/SLAC I ran a high-throughput
synthesis lab producing thin-film and bulk compositionally complex alloys,
integrating theory, synthesis, and characterization into one feedback loop.

### Breadth across synthesis and characterization

Sputtering targets, printed metal, synchrotron beamlines, electron
microscopes — I've spent a career getting hands-on with the instruments
before trying to automate them. Combinatorial sputtering and physical vapor
deposition, additive manufacturing, X-ray diffraction and tomography, SEM,
EBSD, spectroscopy, and *in situ* characterization designed from scratch for
experiments nobody had run before. That breadth is exactly why the
automation work holds up — it's hard to write a good tool for an instrument
you've never had to fix yourself.

## In the field

<div class="photo-gallery">
  <figure>
    <img src="/img/portfolio/agentic-framework-talk.jpg" alt="Presenting my research at MRS Spring 2026.">
    <figcaption>Presenting the agentic framework behind our self-driving Zeiss Versa X-ray microscope — planning, tool use, and a knowledge database wired straight into the instrument.</figcaption>
  </figure>
  <figure>
    <img src="/img/portfolio/ssrl-beamline.jpg" alt="Standing awkwardly next to the first beamline instrument I designed and implemented.">
    <figcaption>Beamline BL 10-2 at SSRL — one of the custom synchrotron end-stations I helped build and run for combinatorial alloy characterization.</figcaption>
  </figure>
  <figure>
    <img src="/img/portfolio/synthesis-lab.png" alt="Working in the high entropy alloy design and discovery lab.">
    <figcaption>Pulling a sample flange in the combinatorial synthesis lab — high-throughput sputtering, before the alloy ever sees a beamline.</figcaption>
  </figure>
</div>

## Experience

<div class="timeline">
  <div class="timeline__item">
    <div class="timeline__when">2026 &ndash; present</div>
    <div class="timeline__what">
      <strong>Senior Scientist, Materials Research</strong> &middot; Carl Zeiss Research Microscopy Solutions
      <p>Leading development of autonomous, self-driving X-ray and electron microscopy systems.</p>
    </div>
  </div>
  <div class="timeline__item">
    <div class="timeline__when">2023 &ndash; 2026</div>
    <div class="timeline__what">
      <strong>Applications Development Scientist</strong> &middot; Carl Zeiss Research Microscopy Solutions
      <p>Architected the agentic systems and instrument tooling this page is mostly about.</p>
    </div>
  </div>
  <div class="timeline__item">
    <div class="timeline__when">2021 &ndash; 2023</div>
    <div class="timeline__what">
      <strong>Postdoctoral Scholar</strong> &middot; Stanford University / SLAC National Accelerator Laboratory
      <p>Ran a high-throughput synthesis lab; integrated active learning and Bayesian design with combinatorial synthesis and custom synchrotron instrumentation.</p>
    </div>
  </div>
  <div class="timeline__item">
    <div class="timeline__when">2018 &ndash; 2021</div>
    <div class="timeline__what">
      <strong>Graduate Research Assistant, ADAPT Fellow</strong> &middot; Los Alamos National Laboratory
      <p>Designed custom in situ X-ray diffraction platforms for additive manufacturing and 3D-printed structures.</p>
    </div>
  </div>
  <div class="timeline__item">
    <div class="timeline__when">2016 &ndash; 2021</div>
    <div class="timeline__what">
      <strong>Ph.D., Materials Science &amp; Engineering</strong> &middot; Colorado School of Mines
      <p>Advised by Dr. Aaron P. Stebner. Novel in situ characterization methods for additive manufacturing.</p>
    </div>
  </div>
  <div class="timeline__item">
    <div class="timeline__when">2012 &ndash; 2016</div>
    <div class="timeline__what">
      <strong>B.A. Physics, Minor in Mathematics</strong> &middot; The College of Wooster
      <p>College Scholar Award; honors thesis.</p>
    </div>
  </div>
</div>

## Technical toolbox

<ul class="skill-chips">
  <li>LLM agents</li>
  <li>Instrument APIs &amp; closed-loop control</li>
  <li>Combinatorial sputtering / PVD</li>
  <li>Additive manufacturing</li>
  <li>X-ray diffraction &amp; tomography</li>
  <li>SEM &amp; EBSD</li>
  <li><em>In situ</em> characterization</li>
  <li>Multi-agent systems</li>
  <li>Planning &amp; tool use</li>
  <li>Structured function calling</li>
  <li>MCP / FastMCP</li>
  <li>LangGraph</li>
  <li>LangChain</li>
  <li>Benchmark &amp; eval harness design</li>
  <li>Python</li>
  <li>Gaussian-process regression</li>
  <li>Active learning</li>
  <li>Computer vision</li>
  <li>Deep-learning image segmentation</li>
</ul>

## Selected publications

<ul class="paper-list">
  <li>
    <a href="/papers/SDLBenchmarks.pdf" target="_blank" rel="noopener">On the Optimization of Architecture, System Hyperparameters, and Context Databases for Agentic Self-Driving Microscopy</a>
    <span class="paper-desc">Manuscript in preparation, 2026</span>
  </li>
  <li>
    <a href="/papers/VGPT.pdf" target="_blank" rel="noopener">Multi-Agent Systems for Autonomous Laboratory Instrument Operation</a>
    <span class="paper-desc">Preprint, 2024</span>
  </li>
  <li>
    <a href="/papers/ALthinfilm.pdf" target="_blank" rel="noopener">Active Learning for Rapid Targeted Synthesis of Compositionally Complex Alloys</a>
    <span class="paper-desc">Materials, vol. 17, no. 16, 2024</span>
  </li>
  <li>
    <a href="/papers/NISTinsitu.pdf" target="_blank" rel="noopener">Accelerating In Situ X-ray Tomography Using Sparse Projections and Deep Learning</a>
    <span class="paper-desc">Materials Characterization, 2026</span>
  </li>
  <li>
    Glass Formation During Combinatorial Sputtering in Binary Alloys
    <span class="paper-desc">S. Huang, N. S. Johnson, et al. &middot; Acta Materialia, vol. 296, 2025</span>
  </li>
</ul>

<p><em>Full list on <a href="https://scholar.google.com/citations?user=MNdLZfwAAAAJ&amp;hl=en" target="_blank" rel="noopener">Google Scholar</a>.</em></p>

## Awards & recognition

<ul class="paper-list">
  <li>
    AIME Champion H. Mathewson Award
    <span class="paper-desc">2024 &middot; for significant contribution to the engineering application of metallic materials</span>
  </li>
  <li>
    Los Alamos ADAPT Advanced Manufacturing Fellowship
    <span class="paper-desc">2018&ndash;2021 &middot; three-year graduate research fellowship</span>
  </li>
  <li>
    Spring Commencement Student Speaker
    <span class="paper-desc">Colorado School of Mines, 2021</span>
  </li>
</ul>

## Let's talk

<p class="cta-row">
  <a class="cta-btn" href="/resume/NathanJohnson_Resume.pdf" target="_blank" rel="noopener">Download resume (PDF)</a>
  <a class="cta-btn cta-btn--ghost" href="mailto:nathan.scott.johnson@gmail.com">Email me</a>
  <a class="cta-btn cta-btn--ghost" href="https://www.linkedin.com/in/nathan-johnson-705656287/" target="_blank" rel="noopener">LinkedIn</a>
</p>
