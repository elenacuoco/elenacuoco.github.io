---
layout: default
title: Projects
permalink: /projects/
toc:
  - name: Software
    anchor: software
---

<div class="page-title">
  <p class="eyebrow">Software</p>
  <h1>Projects</h1>
  <p class="subtitle">
    Open-source tools for gravitational-wave data analysis and signal detection.
  </p>
</div>

<section class="home-section" id="software">
  <h2>Software</h2>

  <div class="feature-grid">
    <div class="feature-card">
      <h3>p4TSA</h3>
      <p>
        A minimal C++ core library, with Python bindings, of ad-hoc functions for
        working with time series — whitening, wavelet decomposition, and
        wavelet-based detection filtering for gravitational-wave detector data.
      </p>
      <a class="btn btn-secondary" href="https://github.com/elenacuoco/p4TSA" target="_blank" rel="noopener">
        GitHub
      </a>
    </div>

    <div class="feature-card">
      <h3>WDFlow</h3>
      <p>
        A standalone Python package implementing the Wavelet Detection Filter (WDF)
        trigger-generation pipeline, built on p4TSA, for real-time detection of
        unmodeled transient signals in gravitational-wave data — with clustering,
        multi-detector coincidence, and false-alarm probability estimation.
      </p>
      <a class="btn btn-secondary" href="https://github.com/elenacuoco/wdflow" target="_blank" rel="noopener">
        GitHub
      </a>
      <a class="btn btn-secondary" href="https://elenacuoco.github.io/wdflow/index.html" target="_blank" rel="noopener">
        Documentation
      </a>
    </div>

    <div class="feature-card">
      <h3>Wavefier</h3>
      <p>
        A framework for multi-messenger astronomy, connecting gravitational-wave
        and electromagnetic observations across the analysis pipeline.
      </p>
      <a class="btn btn-secondary" href="https://github.com/wavefier" target="_blank" rel="noopener">
        GitHub
      </a>
      <a class="btn btn-secondary" href="https://wavefier.github.io/wavefier/" target="_blank" rel="noopener">
        Documentation
      </a>
    </div>
  </div>
</section>
