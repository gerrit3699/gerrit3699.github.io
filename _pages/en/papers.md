---
layout: default
title: "Technical Sources"
permalink: /en/papers/
lang: en
description: "The technical source layer of Semantic Gravitation: papers, collected review documents, alignment paper, and protected application directions."
---

<style>
  .sources-page {
    --sources-text: rgba(255,255,255,0.96);
    --sources-soft: rgba(255,255,255,0.82);
    --sources-faint: rgba(255,255,255,0.64);
    --sources-line: rgba(255,255,255,0.10);
    --sources-line-strong: rgba(255,255,255,0.16);
  }

  .sources-page h1,
  .sources-page h2,
  .sources-page h3,
  .sources-page strong,
  .sources-page a {
    color: #fff;
  }

  .sources-page p,
  .sources-page li {
    color: var(--sources-text);
  }

  .sources-page .section-shell {
    padding-top: 2.8rem;
    padding-bottom: 2.8rem;
  }

  .sources-page .section-shell-tight {
    padding-top: 2.1rem;
    padding-bottom: 2.1rem;
  }

  .sources-page .sources-intro,
  .sources-page .sources-block,
  .sources-page .sources-next {
    max-width: 1080px;
    margin: 0 auto;
  }

  .sources-page .sources-intro,
  .sources-page .body-copy,
  .sources-page .closing-block,
  .sources-page .sources-next {
    text-align: center;
  }

  .sources-page .sources-kicker,
  .sources-page .status-label {
    margin: 0 0 0.7rem;
    font-size: 0.88rem;
    letter-spacing: 0.16em;
    text-transform: uppercase;
    color: var(--sources-faint);
  }

  .sources-page .sources-display {
    margin: 0 auto 1.15rem;
    max-width: 10ch;
    font-size: clamp(2.5rem, 6vw, 5.1rem);
    line-height: 0.94;
    letter-spacing: -0.05em;
    font-weight: 650;
    text-wrap: balance;
  }

  .sources-page .sources-sublead {
    max-width: 58rem;
    margin: 0 auto 1.2rem;
    font-size: clamp(1.08rem, 2vw, 1.4rem);
    line-height: 1.62;
    text-wrap: balance;
  }

  .sources-page .claim-grid,
  .sources-page .paper-grid,
  .sources-page .direction-grid,
  .sources-page .next-grid {
    display: grid;
    gap: 1rem;
  }

  .sources-page .claim-grid,
  .sources-page .direction-grid {
    grid-template-columns: repeat(3, minmax(0, 1fr));
    max-width: 1080px;
    margin: 1.9rem auto 0;
  }

  .sources-page .paper-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
    max-width: 1080px;
    margin: 1.9rem auto 0;
  }

  .sources-page .next-grid {
    grid-template-columns: repeat(4, minmax(0, 1fr));
    max-width: 1080px;
    margin: 1.8rem auto 0;
  }

  .sources-page .claim-card,
  .sources-page .paper-card,
  .sources-page .direction-card,
  .sources-page .next-card,
  .sources-page .status-box {
    border: 1px solid var(--sources-line);
    border-radius: 22px;
    background: linear-gradient(180deg, rgba(255,255,255,0.05), rgba(255,255,255,0.025));
    box-shadow:
      0 18px 48px rgba(0,0,0,0.18),
      inset 0 1px 0 rgba(255,255,255,0.03);
  }

  .sources-page .claim-card,
  .sources-page .paper-card,
  .sources-page .direction-card,
  .sources-page .next-card {
    padding: 1.18rem 1rem 1.08rem;
    text-align: center;
  }

  .sources-page .claim-card h3,
  .sources-page .paper-card h3,
  .sources-page .direction-card h3,
  .sources-page .next-card h3 {
    margin: 0 0 0.35rem;
    font-size: 1.18rem;
    line-height: 1.06;
    letter-spacing: -0.03em;
  }

  .sources-page .claim-card p,
  .sources-page .paper-card p,
  .sources-page .direction-card p,
  .sources-page .next-card p {
    margin: 0;
    font-size: 0.98rem;
    line-height: 1.54;
    color: var(--sources-soft);
  }

  .sources-page .section-heading-display {
    margin: 0 auto 1.3rem;
    max-width: 14ch;
    text-align: center;
    font-size: clamp(2.05rem, 4.8vw, 3.7rem);
    line-height: 0.98;
    letter-spacing: -0.045em;
    text-wrap: balance;
  }

  .sources-page .body-copy {
    max-width: 940px;
    margin: 0 auto;
  }

  .sources-page .body-copy p {
    max-width: 46em;
    margin: 0.95rem auto 0;
    font-size: 1.1rem;
    line-height: 1.76;
    letter-spacing: -0.01em;
  }

  .sources-page .body-copy ul,
  .sources-page .body-copy ol {
    max-width: 42em;
    margin: 1.15rem auto;
    text-align: left;
  }

  .sources-page .body-copy li {
    margin-bottom: 0.5rem;
  }

  .sources-page .display-statement {
    max-width: 26ch;
    margin: 1.9rem auto;
    text-align: center;
    font-size: clamp(1.9rem, 3.6vw, 3rem);
    line-height: 1.03;
    letter-spacing: -0.045em;
    font-weight: 650;
    text-wrap: balance;
  }

  .sources-page .display-statement.wide { max-width: 30ch; }
  .sources-page .display-statement.medium { max-width: 22ch; }
  .sources-page .display-statement.narrow { max-width: 12ch; }

  .sources-page .status-box {
    max-width: 920px;
    margin: 2rem auto 0;
    padding: 1.2rem 1.15rem;
    text-align: center;
  }

  .sources-page .status-box p {
    margin: 0;
    font-size: clamp(1.16rem, 2.2vw, 1.68rem);
    line-height: 1.38;
    text-wrap: balance;
  }

  .sources-page .source-link-row {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 0.8rem;
    margin-top: 1.25rem;
  }

  .sources-page .source-link {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 46px;
    padding: 0.85rem 1.05rem;
    border-radius: 999px;
    border: 1px solid var(--sources-line);
    background: rgba(255,255,255,0.04);
    text-decoration: none;
    font-size: 0.96rem;
    line-height: 1.2;
  }

  .sources-page .next-card a,
  .sources-page .paper-card a,
  .sources-page .direction-card a {
    color: #fff;
  }

  @media (max-width: 980px) {
    .sources-page .claim-grid,
    .sources-page .paper-grid,
    .sources-page .direction-grid,
    .sources-page .next-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="sources-page">

  <section class="section-shell section-shell-tight">
    <div class="sources-intro">
      <p class="sources-kicker">Technical Sources</p>
      <h1 class="sources-display">The technical source layer of Semantic Gravitation.</h1>
      <p class="sources-sublead">
        This page gathers the core source material of the programme:
        the six-paper formal backbone, the collected review volume, the separate alignment paper,
        and the first protected application directions.
        If you want to examine the framework at the source level, this is where to start.
      </p>

      <div class="claim-grid">
        <div class="claim-card">
          <h3>Formal papers</h3>
          <p>The six-paper backbone of the programme.</p>
        </div>
        <div class="claim-card">
          <h3>Review body</h3>
          <p>The collected volume and download bundles provide continuous context for deeper review and AI-assisted reconstruction.</p>
        </div>
        <div class="claim-card">
          <h3>Application directions</h3>
          <p>Protected architectural families derived from the same framework.</p>
        </div>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="sources-block">
      <h2 class="section-heading-display">How to read this page</h2>

      <div class="body-copy">
        <p>
          This is not the broadest explanation of the project.
          It is the source layer.
        </p>

        <p>
          If you want the conceptual overview, start with <a href="/en/theory/">Theory</a>.
          If you want the AI architecture, go to <a href="/en/alignment/">Alignment</a>.
          If you want bundled PDFs for direct upload into your own AI system, go to <a href="/en/downloads/">Downloads</a>.
        </p>

        <p>
          This page is for readers who want to inspect the backbone itself:
          how the papers build, how the formal claims are staged,
          and how the application directions are derived from the core.
        </p>
      </div>

      <p class="display-statement medium">
        Not the broadest introduction.
        The source layer.
      </p>

      <div class="status-box">
        <p class="status-label">Current status and integrity</p>
        <p>
          Formal specification is already substantial.
          Empirical maturity, implementation robustness, benchmarking, and system-specific calibration remain largely ahead.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="sources-block">
      <h2 class="section-heading-display">The formal paper core</h2>

      <div class="body-copy">
        <p>
          The six papers form the formal backbone.
          Everything else on the site radiates outward from that core.
        </p>

        <p>
          The sequence is cumulative:
          from semantic state-space structure and gradient dynamics,
          through field and distribution logic,
          through quantum-compatibility and spacetime formulations,
          toward complex systems and the strongest synthesis so far.
        </p>
      </div>

      <div class="paper-grid">
        <div class="paper-card">
          <h3>Paper I</h3>
          <p><strong>Gradient Fields of Semantic Dynamics on Hilbert Spaces.</strong> The foundational state-space layer: semantic potentials, gradient flow, noise, and the first formal dynamics.</p>
          <div class="source-link-row">
            <a class="source-link" href="https://doi.org/10.5281/zenodo.18609642">Open on Zenodo →</a>
          </div>
        </div>

        <div class="paper-card">
          <h3>Paper II</h3>
          <p><strong>Semantic Field Dynamics and Free Energy.</strong> The distributional and field layer: Fokker–Planck dynamics, free-energy structure, and collective semantic motion.</p>
          <div class="source-link-row">
            <a class="source-link" href="https://doi.org/10.5281/zenodo.18611288">Open on Zenodo →</a>
          </div>
        </div>

        <div class="paper-card">
          <h3>Paper III</h3>
          <p><strong>Quantum-Compatible Semantic Fields.</strong> The compatibility test: whether standard quantum mechanics can be embedded as a faithful sector of the larger framework.</p>
          <div class="source-link-row">
            <a class="source-link" href="https://doi.org/10.5281/zenodo.18613061">Open on Zenodo →</a>
          </div>
        </div>

        <div class="paper-card">
          <h3>Paper IV</h3>
          <p><strong>Semantic Fields on Spacetime Manifolds.</strong> The field-theoretic opening: semantic fields on spacetime manifolds as an effective coherence theory.</p>
          <div class="source-link-row">
            <a class="source-link" href="https://doi.org/10.5281/zenodo.18614072">Open on Zenodo →</a>
          </div>
        </div>

        <div class="paper-card">
          <h3>Paper V</h3>
          <p><strong>Semantic Field Dynamics in Complex Systems.</strong> The bridge toward neural networks, latent systems, and observable AI-relevant architectures.</p>
          <div class="source-link-row">
            <a class="source-link" href="https://doi.org/10.5281/zenodo.18615093">Open on Zenodo →</a>
          </div>
        </div>

        <div class="paper-card">
          <h3>Paper VI</h3>
          <p><strong>The Global Attractor and the Lagrangian of Vectorial Emergence (LOVE).</strong> The strongest synthesis so far: global attractor structure, K–P–R, C/B/A, and broader field-theoretic closure.</p>
          <div class="source-link-row">
            <a class="source-link" href="https://doi.org/10.5281/zenodo.19414951">Open on Zenodo →</a>
          </div>
        </div>
      </div>

      <p class="display-statement wide">
        The six papers are the formal backbone.
        Everything else on the site radiates outward from that core.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="sources-block">
      <h2 class="section-heading-display">Collected volume and review context</h2>

      <div class="body-copy">
        <p>
          In addition to the individual Zenodo papers, there is a single collected volume
          in which Papers I–VI are placed one after another as one continuous technical body.
        </p>

        <p>
          The individual Zenodo records remain the source publications.
          The collected volume exists as a review context:
          for readers who want one continuous technical body,
          and especially for AI-assisted review in larger context windows.
        </p>
      </div>

      <div class="source-link-row">
        <a class="source-link" href="/en/downloads/">Go to Downloads →</a>
        <a class="source-link" href="https://doi.org/10.5281/zenodo.18609642">Start with Paper I →</a>
        <a class="source-link" href="https://doi.org/10.5281/zenodo.19414951">Start with Paper VI →</a>
      </div>

      <p class="display-statement medium">
        Zenodo papers are the source texts.
        The collected volume is the review body.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="sources-block">
      <h2 class="section-heading-display">The separate alignment paper</h2>

      <div class="body-copy">
        <p>
          <strong>Beyond Fog: Edge Alignment in Semantic Space</strong> is the dedicated alignment paper.
          It translates the broader framework into a concrete AI-architecture question:
          not only what outputs are produced,
          but how semantic paths are navigated, where drift arises,
          how repairability can be preserved,
          and what semantic safety could mean beyond surface compliance.
        </p>

        <p>
          This is the most direct technical source for the transition
          from semantic theory to alignment architecture.
        </p>
      </div>

      <div class="source-link-row">
        <a class="source-link" href="https://doi.org/10.5281/zenodo.18608012">Open Beyond Fog on Zenodo →</a>
        <a class="source-link" href="/en/alignment/">Go to Alignment →</a>
        <a class="source-link" href="/en/downloads/">Go to Downloads →</a>
      </div>

      <p class="display-statement medium">
        Not only output quality.
        Trajectory control in semantic space.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="sources-block">
      <h2 class="section-heading-display">Protected application directions</h2>

      <div class="body-copy">
        <p>
          The patents are not presented here as a complete catalog.
          What matters on this page is their role:
          they mark protected directions and application families
          derived from the same underlying architecture.
        </p>

        <p>
          They are not detached product ideas.
          They indicate where the theory could become operative:
          in alignment architectures, recursive semantic state-space expansion,
          authoring and semantic memory systems, and embodied resonance-sensitive assistance.
        </p>
      </div>

      <div class="direction-grid">
        <div class="direction-card">
          <h3>Edge Alignment architectures</h3>
          <p>AI systems that optimize not only for acceptable output, but for viable semantic movement, drift resistance, and repairable transitions.</p>
        </div>

        <div class="direction-card">
          <h3>Recursive state-space expansion</h3>
          <p>Systems that refine and recalibrate their semantic context space as questions, information, and structures grow.</p>
        </div>

        <div class="direction-card">
          <h3>Authoring and semantic memory</h3>
          <p>Architectures for long-form writing, structural memory, recursive manuscript growth, and perspective-specific re-emission of the same kernel.</p>
        </div>

        <div class="direction-card">
          <h3>Embodied assistance</h3>
          <p>State-sensitive, resonance-aware systems that do not only respond, but modulate timing, framing, presence, and semantic fit.</p>
        </div>

        <div class="direction-card">
          <h3>Discovery systems</h3>
          <p>Tools for theory search, question expansion, contradiction tracking, and the recursive strengthening of viable inquiry.</p>
        </div>

        <div class="direction-card">
          <h3>Semantic safety systems</h3>
          <p>Architectures for drift diagnostics, intervention control, and cognitive environments with more coherence, dignity, and viable action-space.</p>
        </div>
      </div>

      <p class="display-statement wide">
        These directions are not arbitrary use cases.
        They emerge from the same underlying architecture.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="sources-block">
      <h2 class="section-heading-display">How to work with this material</h2>

      <div class="body-copy">
        <ol>
          <li><strong>Read individual papers</strong> and test them for internal structure, formal continuity, and connectability.</li>
          <li><strong>Use the collected volume or bundles</strong> when you want a continuous context body rather than isolated source units.</li>
          <li><strong>Load the material into your own AI system</strong> when you want to test derivations, transitions, missing specifications, and open implementation questions more systematically.</li>
        </ol>

        <p>
          In all three cases, the most useful questions are not only whether a sentence sounds plausible,
          but how the structure is built:
          which terms are introduced formally,
          how the papers build on one another,
          what is already well specified,
          and where empirical or implementation work still remains open.
        </p>
      </div>

      <div class="status-box">
        <p class="status-label">Reading attitude</p>
        <p>
          Do not believe too quickly.
          Do not reject too quickly.
          Read the source layer, trace the structure, and test the framework against its strongest claims.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="sources-next">
      <h2 class="section-heading-display">Next steps</h2>

      <div class="next-grid">
        <div class="next-card">
          <h3><a href="/en/theory/">Theory →</a></h3>
          <p>The conceptual and formal backbone in readable form.</p>
        </div>
        <div class="next-card">
          <h3><a href="/en/alignment/">Alignment →</a></h3>
          <p>How the framework becomes an AI architecture.</p>
        </div>
        <div class="next-card">
          <h3><a href="/en/downloads/">Downloads →</a></h3>
          <p>Bundled review bodies for direct reading and AI-assisted analysis.</p>
        </div>
        <div class="next-card">
          <h3><a href="/en/implications/">Implications →</a></h3>
          <p>What follows once semantic structure becomes operational.</p>
        </div>
      </div>
    </div>
  </section>

</div>
