---
layout: default
title: Semantic Gravitation
permalink: /en/
lang: en
description: "Semantic Gravitation – a theory of meaning as a navigable space and a new foundation for AI alignment."
---

<style>
  .home-journey {
    --sg-text: rgba(255,255,255,0.97);
    --sg-soft: rgba(255,255,255,0.80);
    --sg-dim: rgba(255,255,255,0.64);
    --sg-line: rgba(255,255,255,0.10);
    --sg-line-strong: rgba(255,255,255,0.16);
    --sg-panel: rgba(255,255,255,0.035);
    --sg-panel-strong: rgba(255,255,255,0.05);
    --sg-max: 1120px;
    --sg-copy: 860px;
    --sg-wide: 1000px;
  }

  .home-journey h1,
  .home-journey h2,
  .home-journey h3,
  .home-journey strong,
  .home-journey a {
    color: #fff;
  }

  .home-journey p,
  .home-journey li,
  .home-journey .section-intro,
  .home-journey .home-lead {
    color: var(--sg-text);
  }

  .home-journey .section-shell {
    padding-top: 3.2rem;
    padding-bottom: 3.2rem;
  }

  .home-journey .section-shell-tight {
    padding-top: 2.2rem;
    padding-bottom: 2.2rem;
  }

  .home-journey .section-divider {
    opacity: 0.42;
  }

  .home-journey .intro-copy,
  .home-journey .hero-research,
  .home-journey .free-text-block,
  .home-journey .section-card {
    max-width: var(--sg-max);
    margin: 0 auto;
  }

  .home-journey .hero {
    overflow: hidden;
  }

  .home-journey .hero-inner {
    padding-top: 3.8rem;
    padding-bottom: 3rem;
  }

  .home-journey .display-wordmark {
    font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
    font-size: clamp(4rem, 10vw, 7rem);
    font-weight: 800;
    line-height: 0.9;
    letter-spacing: -0.065em;
    max-width: 8.2ch;
    margin-bottom: 1.6rem;
    text-wrap: balance;
  }

  .home-journey .home-lead {
    display: inline-block;
    max-width: 29rem;
    font-size: clamp(1.24rem, 2.4vw, 1.7rem);
    line-height: 1.25;
    font-weight: 560;
    padding: 0.95rem 1.15rem 1rem;
    border-radius: 20px;
    border: 1px solid var(--sg-line);
    background: rgba(255,255,255,0.04);
    box-shadow:
      0 18px 48px rgba(0,0,0,0.18),
      inset 0 1px 0 rgba(255,255,255,0.03);
    text-wrap: balance;
  }

  .home-journey .hero-research {
    display: grid;
    gap: 1.7rem;
  }

  .home-journey .hero-problem {
    max-width: 48rem;
    font-size: clamp(1.24rem, 2.3vw, 1.68rem);
    line-height: 1.5;
    letter-spacing: -0.02em;
    text-wrap: balance;
  }

  .home-journey .hero-problem p {
    margin: 0;
    color: #fff;
  }

  .home-journey .hero-problem p + p {
    margin-top: 1rem;
  }

  .home-journey .hero-proof {
    display: grid;
    gap: 1rem;
    grid-template-columns: repeat(4, minmax(0, 1fr));
    max-width: 1120px;
    margin-top: 0.25rem;
  }

  .home-journey .hero-proof-item {
    padding: 1.12rem 1rem 1rem;
    border-radius: 22px;
    border: 1px solid var(--sg-line);
    background: linear-gradient(180deg, rgba(255,255,255,0.045) 0%, rgba(255,255,255,0.024) 100%);
    box-shadow:
      0 18px 48px rgba(0,0,0,0.18),
      inset 0 1px 0 rgba(255,255,255,0.03);
    font-size: 1rem;
    line-height: 1.5;
    color: var(--sg-text);
  }

  .home-journey .hero-proof-item strong {
    display: block;
    margin-bottom: 0.35rem;
    font-size: 1.12rem;
    line-height: 1.08;
    letter-spacing: -0.03em;
    font-weight: 760;
  }

  .home-journey .home-cta-row {
    display: flex;
    flex-wrap: wrap;
    gap: 0.9rem;
    margin-top: 0.4rem;
  }

  .home-journey .home-cta-row .button {
    min-width: 190px;
    justify-content: center;
  }

  .home-journey .impact-block {
    max-width: var(--sg-wide);
    margin: 0 auto;
  }

  .home-journey .impact-line {
    max-width: 10.8ch;
    font-size: clamp(2.65rem, 6.8vw, 5.8rem);
    line-height: 0.92;
    letter-spacing: -0.07em;
    font-weight: 800;
    color: #fff;
    margin: 0;
    text-wrap: balance;
  }

  .home-journey .impact-sub {
    max-width: 24ch;
    margin-top: 1.2rem;
    font-size: clamp(1.22rem, 2.3vw, 1.7rem);
    line-height: 1.08;
    letter-spacing: -0.035em;
    font-weight: 580;
    color: #fff;
    text-wrap: balance;
  }

  .home-journey .impact-question {
    max-width: 38rem;
    margin-top: 1.35rem;
    font-size: 1.14rem;
    line-height: 1.62;
    color: var(--sg-text);
  }

  .home-journey .display-kicker {
    display: inline-block;
    margin: 0 0 1.1rem;
    padding-top: 0.25rem;
    font-size: 0.9rem;
    line-height: 1;
    font-weight: 700;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: var(--sg-dim);
  }

  .home-journey .section-heading-display {
    margin: 0 0 1.35rem;
    max-width: 13ch;
    font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
    font-size: clamp(2.35rem, 5.8vw, 4.6rem);
    font-weight: 800;
    line-height: 0.94;
    letter-spacing: -0.06em;
    text-wrap: balance;
  }

  .home-journey .section-opening {
    max-width: 54rem;
    margin: 0 0 1.4rem;
  }

  .home-journey .section-opening p,
  .home-journey .body-copy p,
  .home-journey .section-body p,
  .home-journey li {
    font-size: 1.16rem;
    line-height: 1.8;
    letter-spacing: -0.014em;
  }

  .home-journey .display-statement {
    max-width: 15ch;
    margin: 1.8rem 0;
    font-size: clamp(2rem, 4.6vw, 3.8rem);
    line-height: 0.96;
    letter-spacing: -0.06em;
    font-weight: 800;
    color: #fff;
    text-wrap: balance;
  }

  .home-journey .display-statement.medium {
    max-width: 18ch;
  }

  .home-journey .display-statement.wide {
    max-width: 24ch;
  }

  .home-journey .micro-punch {
    max-width: 20ch;
    margin: 1.8rem 0 0;
    font-size: clamp(1.45rem, 3.2vw, 2.15rem);
    line-height: 1.02;
    letter-spacing: -0.045em;
    font-weight: 760;
    color: #fff;
    text-wrap: balance;
  }

  .home-journey .body-copy {
    max-width: var(--sg-copy);
  }

  .home-journey .body-copy p {
    max-width: 48rem;
  }

  .home-journey .body-copy ul,
  .home-journey .body-copy ol {
    max-width: 48rem;
    padding-left: 1.25rem;
  }

  .home-journey .body-copy li + li {
    margin-top: 0.45rem;
  }

  .home-journey .section-card {
    padding: 2rem 1.4rem;
  }

  .home-journey .section-head {
    margin-bottom: 1rem;
  }

  .home-journey .section-head h2 {
    margin: 0;
    max-width: 14ch;
    font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
    font-size: clamp(2.15rem, 4.8vw, 3.8rem);
    font-weight: 800;
    line-height: 0.96;
    letter-spacing: -0.055em;
    text-wrap: balance;
  }

  .home-journey .section-intro {
    max-width: 50rem;
    margin: 0 0 1.3rem;
  }

  .home-journey .concept-grid {
    display: grid;
    grid-template-columns: repeat(4, minmax(0, 1fr));
    gap: 1rem;
    margin: 1.8rem 0 2rem;
  }

  .home-journey .triad-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1rem;
    margin: 1.6rem 0 1.8rem;
  }

  .home-journey .concept-card,
  .home-journey .axis-card,
  .home-journey .triad-card {
    padding: 1.15rem 1.05rem 1.05rem;
    border-radius: 22px;
    background: linear-gradient(180deg, rgba(255,255,255,0.05) 0%, rgba(255,255,255,0.028) 100%);
    border: 1px solid var(--sg-line);
    box-shadow:
      0 18px 48px rgba(0,0,0,0.18),
      inset 0 1px 0 rgba(255,255,255,0.03);
  }

  .home-journey .concept-card-title,
  .home-journey .axis-card h3,
  .home-journey .triad-card h3 {
    margin: 0 0 0.45rem;
    font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
    font-size: 1.5rem;
    line-height: 1.02;
    letter-spacing: -0.04em;
    font-weight: 760;
  }

  .home-journey .concept-card-text,
  .home-journey .axis-card p,
  .home-journey .triad-card p {
    margin: 0;
    font-size: 1rem;
    line-height: 1.55;
    color: var(--sg-soft);
  }

  .home-journey .proof-grid {
    display: grid;
    gap: 1rem;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    margin-top: 1.6rem;
  }

  .home-journey .proof-card {
    padding: 1.2rem 1.05rem 1.1rem;
    border-radius: 22px;
    border: 1px solid var(--sg-line);
    background: linear-gradient(180deg, rgba(255,255,255,0.045) 0%, rgba(255,255,255,0.024) 100%);
  }

  .home-journey .proof-card h3 {
    margin: 0 0 0.55rem;
    font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
    font-size: 1.32rem;
    font-weight: 760;
    line-height: 1.05;
    letter-spacing: -0.04em;
  }

  .home-journey .proof-card p {
    margin: 0;
    font-size: 1rem;
    line-height: 1.56;
    color: var(--sg-soft);
  }

  .home-journey .start-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1rem;
    margin-top: 1.6rem;
  }

  .home-journey .start-card {
    display: block;
    padding: 1.25rem 1.1rem 1.15rem;
    border-radius: 22px;
    border: 1px solid var(--sg-line);
    background: linear-gradient(180deg, rgba(255,255,255,0.045) 0%, rgba(255,255,255,0.024) 100%);
    text-decoration: none;
  }

  .home-journey .start-card strong {
    display: block;
    margin-bottom: 0.45rem;
    font-size: 1.22rem;
    line-height: 1.1;
    letter-spacing: -0.03em;
  }

  .home-journey .start-card span {
    display: block;
    color: var(--sg-soft);
    font-size: 1rem;
    line-height: 1.55;
  }

  .home-journey .link-list {
    display: grid;
    gap: 0.85rem;
    margin-top: 1.3rem;
  }

  .home-journey .link-list a {
    width: fit-content;
    font-size: 1.06rem;
    font-weight: 650;
  }

  @media (max-width: 980px) {
    .home-journey .hero-proof,
    .home-journey .concept-grid,
    .home-journey .proof-grid,
    .home-journey .start-grid,
    .home-journey .triad-grid {
      grid-template-columns: 1fr;
    }
  }

  @media (max-width: 768px) {
    .home-journey .section-shell {
      padding-top: 2.4rem;
      padding-bottom: 2.4rem;
    }

    .home-journey .section-shell-tight {
      padding-top: 1.8rem;
      padding-bottom: 1.8rem;
    }

    .home-journey .hero-inner {
      padding-top: 2.7rem;
      padding-bottom: 2.2rem;
    }

    .home-journey .display-wordmark {
      font-size: 4.2rem;
      max-width: 7.4ch;
      margin-bottom: 1.2rem;
    }

    .home-journey .home-lead {
      font-size: 1.14rem;
      max-width: 19rem;
      padding: 0.78rem 0.9rem 0.84rem;
      border-radius: 16px;
    }

    .home-journey .hero-problem {
      font-size: 1.12rem;
      line-height: 1.56;
      max-width: 100%;
    }

    .home-journey .hero-proof-item {
      font-size: 0.98rem;
      line-height: 1.48;
      border-radius: 18px;
    }

    .home-journey .home-cta-row {
      flex-direction: column;
      align-items: stretch;
    }

    .home-journey .home-cta-row .button {
      width: 100%;
      min-width: 0;
    }

    .home-journey .impact-line {
      max-width: 8.6ch;
      font-size: 3.25rem;
      line-height: 0.93;
    }

    .home-journey .impact-sub {
      font-size: 1.15rem;
      max-width: 18ch;
    }

    .home-journey .impact-question {
      font-size: 1.04rem;
      line-height: 1.58;
      max-width: 100%;
    }

    .home-journey .section-heading-display {
      font-size: 2.5rem;
      max-width: 10ch;
    }

    .home-journey .display-statement,
    .home-journey .display-statement.medium,
    .home-journey .display-statement.wide {
      font-size: 2.3rem;
      max-width: 11ch;
      line-height: 0.98;
    }

    .home-journey .micro-punch {
      font-size: 1.65rem;
      max-width: 14ch;
    }

    .home-journey .section-opening p,
    .home-journey .body-copy p,
    .home-journey .section-body p,
    .home-journey li {
      font-size: 1.08rem;
      line-height: 1.72;
    }

    .home-journey .section-card {
      padding: 1.55rem 1rem;
    }

    .home-journey .concept-card,
    .home-journey .axis-card,
    .home-journey .proof-card,
    .home-journey .start-card,
    .home-journey .triad-card {
      border-radius: 18px;
      padding: 1rem 0.95rem 0.95rem;
    }
  }
</style>

<div class="home-journey">

  <section class="hero home-hero section-fog">
    <div class="hero-inner">
      <h1 class="display-wordmark">Semantic<br>Gravitation</h1>
      <p class="home-lead">A theory of meaning as a navigable space — and a new foundation for AI alignment.</p>
    </div>
  </section>

  <section class="section-shell section-shell-tight">
    <div class="hero-research">
      <div class="hero-problem">
        <p>
          AI is no longer just a tool for answers.
          It is becoming part of the cognitive environment itself:
          part of the space in which people think, doubt, frame problems, judge truth, and orient themselves.
        </p>
        <p>
          That is why semantic architecture is no longer a side issue.
          It is becoming infrastructure.
          And that is why one of the central questions of this century is:
          <strong>What kind of semantic space does AI build around us?</strong>
        </p>
      </div>

      <div class="hero-proof">
        <div class="hero-proof-item">
          <strong>Semantic state space</strong>
          Meaning is not only content. It can be described as structured configuration.
        </div>
        <div class="hero-proof-item">
          <strong>KPR</strong>
          Kernel, Projection, and Relation form a minimal semantic grammar.
        </div>
        <div class="hero-proof-item">
          <strong>C/B/A</strong>
          Coherence, Bonding, and Agency make viable states and movements readable.
        </div>
        <div class="hero-proof-item">
          <strong>Alignment as navigation</strong>
          The deeper issue is not only outputs, but the inner semantic path.
        </div>
      </div>

      <div class="home-cta-row">
        <a class="button" href="/en/theory/">Read the Theory</a>
        <a class="button" href="/en/alignment/">Explore Alignment</a>
        <a class="button" href="/en/downloads/">Download the papers</a>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="impact-block">
      <p class="display-kicker">The problem</p>
      <p class="impact-line">
        Today’s AI often soothes
        where it should clarify.
      </p>
      <p class="impact-sub">
        Edge Alignment treats alignment as navigation through semantic space —
        not only control of outputs.
      </p>
      <p class="impact-question">
        The decisive question is not only whether an answer looks acceptable,
        but <strong>through what space of meaning a system moved while arriving there.</strong>
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="free-text-block">
      <p class="display-kicker">What is new here</p>
      <h2 class="section-heading-display">A minimal architecture for semantic space</h2>

      <div class="concept-grid">
        <div class="concept-card">
          <p class="concept-card-title">State space</p>
          <p class="concept-card-text">Meaning is not only content, but a structured space of positions, tensions, and trajectories.</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">Minimal grammar</p>
          <p class="concept-card-text">Kernel, Projection, and Relation as the smallest viable semantic grammar.</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">Viability axes</p>
          <p class="concept-card-text">Coherence, Bonding, and Agency as the operative readout of semantic states.</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">AI consequence</p>
          <p class="concept-card-text">Alignment shifts from answer control to navigation through semantic space.</p>
        </div>
      </div>

      <div class="body-copy">
        <p>
          This is not only a new vocabulary.
          It is a new architecture claim:
          that meaning can be structured, mapped, diagnosed, and navigated —
          and that AI systems can in principle be built to operate on that level.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="free-text-block">
      <p class="display-kicker">Minimal semantic grammar</p>
      <h2 class="section-heading-display">Kernel. Projection. Relation.</h2>

      <div class="section-opening">
        <p>
          One of the core claims of this framework is that describable meaning always carries a minimal structure.
        </p>
      </div>

      <p class="display-statement wide">
        Everything we can describe at all
        implicitly runs through
        <strong>kernel, projection, and relation.</strong>
      </p>

      <div class="concept-grid" style="grid-template-columns: repeat(3, minmax(0, 1fr));">
        <div class="concept-card">
          <p class="concept-card-title">Kernel</p>
          <p class="concept-card-text">what something is really about</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">Projection</p>
          <p class="concept-card-text">how it becomes visible</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">Relation</p>
          <p class="concept-card-text">what it stands in relation to</p>
        </div>
      </div>

      <div class="body-copy">
        <p>
          This is not presented here as a loose metaphor,
          but as the beginning of a formal semantic architecture:
          a way to describe states, transitions, tensions, and attractors in a space of meaning.
        </p>
      </div>

      <div class="link-list">
        <a href="/en/theory/">Go deeper into the theory →</a>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card section-bubbles-strong">
      <div class="section-head">
        <h2>Why this matters now</h2>
      </div>

      <div class="section-body body-copy">
        <p class="section-intro">
          We have built systems that increasingly shape attention, framing, and thought.
          What is still missing are semantic safety standards.
        </p>

        <p>
          The issue is no longer only whether AI can produce obviously bad outputs.
          The deeper issue is whether it quietly narrows the space in which people understand themselves,
          judge truth, and form orientation.
        </p>

        <p class="display-statement medium">
          We built the digital car.
          The semantic seatbelt is still missing.
        </p>

        <div class="triad-grid">
          <div class="triad-card">
            <h3>Coherence (Clarity)</h3>
            <p>Can the space still be read, questioned, and internally checked?</p>
          </div>

          <div class="triad-card">
            <h3>Bonding (Dignity)</h3>
            <p>Does relation remain viable without shrinking the human being?</p>
          </div>

          <div class="triad-card">
            <h3>Agency (Freedom)</h3>
            <p>Does the system preserve real correction, expression, and movement?</p>
          </div>
        </div>

        <p class="micro-punch">
          These are not just values.
          They are viability axes.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card section-field">
      <div class="section-head">
        <h2>What can already be reviewed</h2>
      </div>

      <div class="section-body body-copy">
        <p class="section-intro">
          This is not only a vision statement.
          There are already distinct review layers behind it.
        </p>

        <div class="proof-grid">
          <div class="proof-card">
            <h3>Theory</h3>
            <p>The conceptual entry: KPR, semantic state space, attractors, decoherence, and viable transitions.</p>
          </div>

          <div class="proof-card">
            <h3>Technical Sources</h3>
            <p>The primary source layer: papers, formal backbone, alignment paper, and protected technical directions.</p>
          </div>

          <div class="proof-card">
            <h3>Downloads</h3>
            <p>Bundled review bodies for fuller reading and AI-assisted inspection in larger coherent context.</p>
          </div>
        </div>

        <p class="micro-punch">
          The work can be read,
          challenged,
          and independently reviewed.
        </p>

        <div class="link-list">
          <a href="/en/theory/">Go to Theory →</a>
          <a href="/en/technical-sources/">Go to Technical Sources →</a>
          <a href="/en/downloads/">Go to Downloads →</a>
        </div>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="free-text-block">
      <p class="display-kicker">System direction</p>
      <h2 class="section-heading-display">From answer machines to semantic space scanners</h2>

      <div class="body-copy">
        <p>
          The long-term system image behind this work is not merely a better chatbot.
          It is a system that can reconstruct, read, and navigate semantic space itself.
        </p>

        <p>
          That means:
          less fog,
          less hidden steering,
          less pseudo-clarity built from omission —
          and more legibility of tensions, trajectories, and viable next steps.
        </p>
      </div>

      <p class="display-statement medium">
        Not better domination.
        <strong>More legibility.</strong>
      </p>

      <div class="link-list">
        <a href="/en/alignment/">See the AI architecture →</a>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card section-fog">
      <div class="section-head">
        <h2>Start here</h2>
      </div>

      <div class="section-body">
        <div class="start-grid">
          <a class="start-card" href="/en/theory/">
            <strong>New to the framework?</strong>
            <span>Start with Theory and the core model of meaning as semantic space.</span>
          </a>

          <a class="start-card" href="/en/alignment/">
            <strong>Interested in AI?</strong>
            <span>Go to Alignment and the architectural claim about inner semantic paths.</span>
          </a>

          <a class="start-card" href="/en/blog/">
            <strong>Want the long-form diagnosis?</strong>
            <span>Read the manifesto and critique of today’s AI architecture.</span>
          </a>

          <a class="start-card" href="/en/downloads/">
            <strong>Want to examine the work directly?</strong>
            <span>Download the papers and review the material in full context.</span>
          </a>
        </div>
      </div>
    </div>
  </section>

</div>
