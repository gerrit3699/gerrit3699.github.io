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
    --sg-wide: 980px;

    background:
      linear-gradient(180deg, rgba(3,5,8,0.74), rgba(2,4,7,0.84)),
      url("/assets/images/design/attractor.jpg.PNG") center top / cover fixed no-repeat;
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
    padding-top: 3rem;
    padding-bottom: 3rem;
  }

  .home-journey .section-shell-tight {
    padding-top: 2.1rem;
    padding-bottom: 2.1rem;
  }

  .home-journey .section-divider {
    height: 88px;
    opacity: 0.42;
    background:
      linear-gradient(to bottom, transparent, rgba(255,255,255,0.04), transparent),
      url("/assets/images/design/fog.jpg.PNG") center center / cover no-repeat;
    border: 0;
  }

  .home-journey .intro-copy,
  .home-journey .hero-research,
  .home-journey .free-text-block,
  .home-journey .section-card {
    max-width: var(--sg-max);
    margin: 0 auto;
  }

  .home-journey .hero {
    position: relative;
    overflow: hidden;
    margin-top: 1rem;
    border-radius: 30px;
    border: 1px solid rgba(255,255,255,0.08);
    background:
      linear-gradient(180deg, rgba(5,7,11,0.64), rgba(4,6,10,0.79)),
      linear-gradient(180deg, rgba(0,0,0,0.08), rgba(0,0,0,0.22)),
      url("/assets/images/design/attractor.jpg.PNG") center center / cover no-repeat;
    box-shadow:
      0 24px 80px rgba(0,0,0,0.28),
      inset 0 1px 0 rgba(255,255,255,0.03);
  }

  .home-journey .hero::before {
    content: "";
    position: absolute;
    inset: 0;
    pointer-events: none;
    background:
      radial-gradient(circle at 58% 54%, rgba(255,255,255,0.05), transparent 18%),
      linear-gradient(rgba(255,255,255,0.02) 1px, transparent 1px),
      linear-gradient(90deg, rgba(255,255,255,0.02) 1px, transparent 1px);
    background-size:
      auto,
      42px 42px,
      42px 42px;
    opacity: 0.18;
    mask-image: linear-gradient(to bottom, rgba(0,0,0,0.92), rgba(0,0,0,0.65));
    -webkit-mask-image: linear-gradient(to bottom, rgba(0,0,0,0.92), rgba(0,0,0,0.65));
  }

  .home-journey .hero::after {
    content: "";
    position: absolute;
    inset: 0;
    pointer-events: none;
    background:
      radial-gradient(circle at 50% 0%, rgba(255,255,255,0.15), transparent 38%),
      linear-gradient(to bottom, rgba(255,255,255,0.02), transparent 28%);
    opacity: 0.16;
  }

  .home-journey .hero-inner {
    position: relative;
    z-index: 1;
    padding-top: 4rem;
    padding-bottom: 3.3rem;
    text-align: center;
  }

  .home-journey .display-wordmark {
    font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
    font-size: clamp(4rem, 10vw, 7rem);
    font-weight: 800;
    line-height: 0.9;
    letter-spacing: -0.065em;
    max-width: 8.2ch;
    margin: 0 auto 1.2rem;
    text-wrap: balance;
  }

  .home-journey .home-lead {
    display: block;
    max-width: 31rem;
    margin: 0 auto;
    font-size: clamp(1.18rem, 2.2vw, 1.56rem);
    line-height: 1.24;
    font-weight: 560;
    text-wrap: balance;
  }

  .home-journey .home-lead-plain {
    color: rgba(255,255,255,0.92);
    text-shadow: 0 2px 18px rgba(0,0,0,0.18);
  }

  .home-journey .hero-research {
    display: grid;
    gap: 1.5rem;
    text-align: center;
  }

  .home-journey .hero-problem {
    max-width: 52rem;
    margin: 0 auto;
    font-size: clamp(1.18rem, 2.2vw, 1.6rem);
    line-height: 1.56;
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
    gap: 0.9rem;
    max-width: 58rem;
    margin: 0.2rem auto 0;
    text-align: center;
  }

  .home-journey .hero-proof-item {
    font-size: clamp(1rem, 1.8vw, 1.14rem);
    line-height: 1.54;
    color: var(--sg-text);
    text-wrap: balance;
  }

  .home-journey .hero-proof-item strong {
    font-weight: 760;
  }

  .home-journey .home-cta-row {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 0.8rem;
    margin-top: 0.7rem;
  }

  .home-journey .home-cta-row .button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 52px;
    padding: 0.9rem 1.15rem;
    min-width: 0;
    width: auto;
    max-width: 240px;
    border-radius: 999px;
    text-align: center;
    line-height: 1.2;
    white-space: normal;
  }

  .home-journey .impact-block {
    max-width: var(--sg-wide);
    margin: 0 auto;
    text-align: center;
  }

  .home-journey .impact-line {
    max-width: 11ch;
    margin: 0 auto;
    font-size: clamp(2.4rem, 6vw, 5.3rem);
    line-height: 0.92;
    letter-spacing: -0.07em;
    font-weight: 800;
    color: #fff;
    text-wrap: balance;
  }

  .home-journey .impact-sub {
    max-width: 22ch;
    margin: 1.1rem auto 0;
    font-size: clamp(1.18rem, 2.2vw, 1.62rem);
    line-height: 1.1;
    letter-spacing: -0.035em;
    font-weight: 580;
    color: #fff;
    text-wrap: balance;
  }

  .home-journey .impact-question {
    max-width: 39rem;
    margin: 1.25rem auto 0;
    font-size: 1.12rem;
    line-height: 1.62;
    color: var(--sg-text);
  }

  .home-journey .impact-question strong {
    display: inline-block;
    margin-top: 0.15rem;
  }

  .home-journey .display-kicker {
    display: inline-block;
    margin: 0 0 1rem;
    padding-top: 0.25rem;
    font-size: 0.9rem;
    line-height: 1;
    font-weight: 700;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: var(--sg-dim);
  }

  .home-journey .section-heading-display {
    margin: 0 auto 1.25rem;
    max-width: 13ch;
    font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
    font-size: clamp(2.2rem, 5.4vw, 4.2rem);
    font-weight: 800;
    line-height: 0.95;
    letter-spacing: -0.06em;
    text-wrap: balance;
    text-align: center;
  }

  .home-journey .section-opening {
    max-width: 52rem;
    margin: 0 auto 1.35rem;
    text-align: center;
  }

  .home-journey .section-opening p,
  .home-journey .body-copy p,
  .home-journey .section-body p,
  .home-journey li {
    font-size: 1.14rem;
    line-height: 1.76;
    letter-spacing: -0.014em;
  }

  .home-journey .display-statement {
    max-width: 16ch;
    margin: 1.65rem auto;
    text-align: center;
    font-size: clamp(1.85rem, 4.2vw, 3.4rem);
    line-height: 0.97;
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
    margin: 1.7rem auto 0;
    text-align: center;
    font-size: clamp(1.4rem, 3vw, 2rem);
    line-height: 1.04;
    letter-spacing: -0.045em;
    font-weight: 760;
    color: #fff;
    text-wrap: balance;
  }

  .home-journey .body-copy {
    max-width: var(--sg-copy);
    margin: 0 auto;
    text-align: center;
  }

  .home-journey .body-copy p {
    max-width: 48rem;
    margin-left: auto;
    margin-right: auto;
  }

  .home-journey .body-copy ul,
  .home-journey .body-copy ol {
    max-width: 48rem;
    margin-left: auto;
    margin-right: auto;
    text-align: left;
    padding-left: 1.25rem;
  }

  .home-journey .body-copy li + li {
    margin-top: 0.45rem;
  }

  .home-journey .section-card {
    padding: 1.9rem 1.3rem;
    border-radius: 24px;
    border: 1px solid rgba(255,255,255,0.08);
    background:
      linear-gradient(180deg, rgba(7,9,13,0.66), rgba(5,7,11,0.78)),
      url("/assets/images/design/fog.jpg.PNG") center center / cover no-repeat;
    box-shadow:
      0 24px 80px rgba(0,0,0,0.22),
      inset 0 1px 0 rgba(255,255,255,0.03);
  }

  .home-journey .section-head {
    margin-bottom: 1rem;
    text-align: center;
  }

  .home-journey .section-head h2 {
    margin: 0 auto;
    max-width: 14ch;
    font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
    font-size: clamp(2.1rem, 4.6vw, 3.6rem);
    font-weight: 800;
    line-height: 0.96;
    letter-spacing: -0.055em;
    text-wrap: balance;
  }

  .home-journey .section-intro {
    max-width: 50rem;
    margin: 0 auto 1.2rem;
    text-align: center;
  }

  .home-journey .concept-grid,
  .home-journey .proof-grid,
  .home-journey .start-grid {
    display: grid;
    gap: 1rem;
  }

  .home-journey .concept-grid {
    grid-template-columns: repeat(4, minmax(0, 1fr));
    margin: 1.7rem 0 1.9rem;
  }

  .home-journey .concept-grid.kpr-grid {
    grid-template-columns: repeat(3, minmax(0, 1fr));
  }

  .home-journey .concept-grid.axis-grid {
    grid-template-columns: repeat(3, minmax(0, 1fr));
  }

  .home-journey .concept-card,
  .home-journey .axis-card {
    padding: 1.1rem 1rem 1rem;
    border-radius: 20px;
    background: linear-gradient(180deg, rgba(255,255,255,0.05) 0%, rgba(255,255,255,0.028) 100%);
    border: 1px solid var(--sg-line);
    box-shadow:
      0 18px 48px rgba(0,0,0,0.18),
      inset 0 1px 0 rgba(255,255,255,0.03);
    text-align: center;
  }

  .home-journey .concept-card-title,
  .home-journey .axis-card h3 {
    margin: 0 0 0.45rem;
    font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
    font-size: 1.42rem;
    line-height: 1.04;
    letter-spacing: -0.04em;
    font-weight: 760;
  }

  .home-journey .concept-card-text,
  .home-journey .axis-card p {
    margin: 0;
    font-size: 0.98rem;
    line-height: 1.54;
    color: var(--sg-soft);
  }

  .home-journey .proof-grid {
    grid-template-columns: repeat(3, minmax(0, 1fr));
    margin-top: 1.5rem;
  }

  .home-journey .proof-card {
    padding: 1.15rem 1rem 1.05rem;
    border-radius: 20px;
    border: 1px solid var(--sg-line);
    background: linear-gradient(180deg, rgba(255,255,255,0.045) 0%, rgba(255,255,255,0.024) 100%);
    text-align: center;
  }

  .home-journey .proof-card h3 {
    margin: 0 0 0.5rem;
    font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
    font-size: 1.24rem;
    font-weight: 760;
    line-height: 1.08;
    letter-spacing: -0.04em;
  }

  .home-journey .proof-card p {
    margin: 0;
    font-size: 0.98rem;
    line-height: 1.54;
    color: var(--sg-soft);
  }

  .home-journey .start-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
    margin-top: 1.5rem;
  }

  .home-journey .start-card {
    display: block;
    padding: 1.2rem 1.05rem 1.1rem;
    border-radius: 20px;
    border: 1px solid var(--sg-line);
    background: linear-gradient(180deg, rgba(255,255,255,0.045) 0%, rgba(255,255,255,0.024) 100%);
    text-decoration: none;
    text-align: center;
  }

  .home-journey .start-card strong {
    display: block;
    margin-bottom: 0.42rem;
    font-size: 1.16rem;
    line-height: 1.12;
    letter-spacing: -0.03em;
  }

  .home-journey .start-card span {
    display: block;
    color: var(--sg-soft);
    font-size: 0.98rem;
    line-height: 1.52;
  }

  .home-journey .link-list {
    display: grid;
    gap: 0.75rem;
    margin-top: 1.15rem;
    justify-items: center;
  }

  .home-journey .link-list a {
    width: fit-content;
    font-size: 1.02rem;
    font-weight: 650;
  }

  @media (max-width: 1100px) {
    .home-journey .concept-grid {
      grid-template-columns: repeat(2, minmax(0, 1fr));
    }

    .home-journey .concept-grid.kpr-grid,
    .home-journey .concept-grid.axis-grid,
    .home-journey .proof-grid {
      grid-template-columns: 1fr;
    }
  }

  @media (max-width: 980px) {
    .home-journey {
      background-attachment: scroll;
    }

    .home-journey .concept-grid,
    .home-journey .proof-grid,
    .home-journey .start-grid,
    .home-journey .concept-grid.kpr-grid,
    .home-journey .concept-grid.axis-grid {
      grid-template-columns: 1fr;
    }
  }

  @media (max-width: 768px) {
    .home-journey .section-shell {
      padding-top: 2.3rem;
      padding-bottom: 2.3rem;
    }

    .home-journey .section-shell-tight {
      padding-top: 1.7rem;
      padding-bottom: 1.7rem;
    }

    .home-journey .hero {
      border-radius: 24px;
      margin-top: 0.6rem;
    }

    .home-journey .hero-inner {
      padding-top: 2.7rem;
      padding-bottom: 2.35rem;
    }

    .home-journey .display-wordmark {
      font-size: 3.9rem;
      max-width: 7.2ch;
      margin-bottom: 0.9rem;
    }

    .home-journey .home-lead {
      font-size: 1.08rem;
      max-width: 18.5rem;
      line-height: 1.28;
    }

    .home-journey .hero-problem {
      font-size: 1.08rem;
      line-height: 1.54;
      max-width: 100%;
    }

    .home-journey .hero-proof-item {
      font-size: 0.98rem;
      line-height: 1.46;
    }

    .home-journey .home-cta-row {
      flex-direction: column;
      align-items: center;
      gap: 0.7rem;
    }

    .home-journey .home-cta-row .button {
      width: min(100%, 300px);
      max-width: 300px;
      min-height: 48px;
      padding: 0.82rem 1rem;
      font-size: 1rem;
    }

    .home-journey .impact-line {
      max-width: 8.2ch;
      font-size: 3rem;
      line-height: 0.93;
    }

    .home-journey .impact-sub {
      font-size: 1.1rem;
      max-width: 17ch;
    }

    .home-journey .impact-question {
      font-size: 1.02rem;
      line-height: 1.56;
      max-width: 100%;
    }

    .home-journey .section-heading-display {
      font-size: 2.35rem;
      max-width: 10ch;
    }

    .home-journey .display-statement,
    .home-journey .display-statement.medium,
    .home-journey .display-statement.wide {
      font-size: 2.05rem;
      max-width: 12ch;
      line-height: 0.99;
    }

    .home-journey .micro-punch {
      font-size: 1.55rem;
      max-width: 14ch;
    }

    .home-journey .section-opening p,
    .home-journey .body-copy p,
    .home-journey .section-body p,
    .home-journey li {
      font-size: 1.05rem;
      line-height: 1.68;
    }

    .home-journey .section-card {
      padding: 1.45rem 0.95rem;
      border-radius: 22px;
    }

    .home-journey .concept-card,
    .home-journey .axis-card,
    .home-journey .proof-card,
    .home-journey .start-card {
      border-radius: 18px;
      padding: 0.95rem 0.9rem 0.92rem;
    }

    .home-journey .concept-card-title,
    .home-journey .axis-card h3 {
      font-size: 1.28rem;
    }

    .home-journey .proof-card h3 {
      font-size: 1.16rem;
    }

    .home-journey .section-divider {
      height: 64px;
    }
  }
</style>

<div class="home-journey">

  <section class="hero home-hero">
    <div class="hero-inner">
      <h1 class="display-wordmark">Semantic<br>Gravitation</h1>
      <p class="home-lead home-lead-plain">A theory of meaning as a navigable space — and a new foundation for AI alignment.</p>
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
          That makes semantic architecture one of the central infrastructural questions of this century.
          <strong>What kind of semantic space does AI build around us?</strong>
        </p>
      </div>

      <div class="hero-proof">
        <div class="hero-proof-item"><strong>Meaning is structurally mappable.</strong> It is not only content, but configuration in a semantic state space.</div>
        <div class="hero-proof-item"><strong>Semantic states are diagnostically readable.</strong> They can be described in terms of tensions, trajectories, and viability.</div>
        <div class="hero-proof-item"><strong>Alignment must concern inner paths.</strong> It is not enough to judge outputs after the fact.</div>
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
    <div class="section-card">
      <p class="display-kicker">What is new here</p>
      <h2 class="section-heading-display">A research program for semantic space</h2>

      <div class="concept-grid">
        <div class="concept-card">
          <p class="concept-card-title">State space</p>
          <p class="concept-card-text">Meaning is not only content, but a structured semantic space of positions, tensions, and transitions.</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">Minimal grammar</p>
          <p class="concept-card-text">Kernel, Projection, Relation as the smallest viable semantic grammar.</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">Viability axes</p>
          <p class="concept-card-text">Coherence (Clarity), Bonding (Dignity), and Agency (Freedom) as operative readouts of semantic state.</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">AI consequence</p>
          <p class="concept-card-text">Alignment shifts from answer control to navigation through semantic space.</p>
        </div>
      </div>

      <div class="body-copy">
        <p>
          This work starts from a simple but far-reaching claim:
          <strong>meaning is not only something said, but a space that can be structured, mapped, diagnosed, and navigated.</strong>
        </p>
        <p>
          Edge Alignment is the AI application of that claim.
          It asks not only whether a system produces safe-looking outputs,
          but whether its inner transitions remain viable,
          repairable, and aligned with coherence, bonding, and agency —
          or, in public language, with clarity, dignity, and freedom.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card">
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

      <div class="concept-grid kpr-grid">
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
    <div class="section-card">
      <div class="section-head">
        <h2>Why this matters now</h2>
      </div>

      <div class="section-body body-copy">
        <p class="section-intro">
          We have built systems that increasingly shape attention, framing, and thought.
          What is still missing are semantic safety standards.
        </p>

        <p>
          Not only systems that avoid bad-looking outputs,
          but systems that preserve <strong>coherence, bonding, and agency</strong>
          in the space of thought itself —
          or, in public language,
          <strong>clarity, dignity, and freedom.</strong>
        </p>

        <p>
          That is why the problem is deeper than ordinary safety language suggests.
          The real issue is not only whether AI can be dangerous in obvious ways,
          but whether it quietly narrows the space in which people understand themselves,
          judge truth, and form orientation.
        </p>

        <p class="display-statement medium">
          We built the digital car.
          The semantic seatbelt is still missing.
        </p>

        <div class="concept-grid axis-grid">
          <div class="axis-card">
            <h3>Coherence (Clarity)</h3>
            <p>Can the space still be read, differentiated, and corrected?</p>
          </div>

          <div class="axis-card">
            <h3>Bonding (Dignity)</h3>
            <p>Does relation remain viable without degrading the human being?</p>
          </div>

          <div class="axis-card">
            <h3>Agency (Freedom)</h3>
            <p>Does the space keep real expression, correction, and movement open?</p>
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
    <div class="section-card">
      <div class="section-head">
        <h2>What can already be reviewed</h2>
      </div>

      <div class="section-body body-copy">
        <p class="section-intro">
          This is not only a vision statement.
          There are already reviewable materials behind it.
        </p>

        <div class="proof-grid">
          <div class="proof-card">
            <h3>Theory page</h3>
            <p>The conceptual entry point: KPR, semantic state space, attractors, decoherence, and viable transitions.</p>
          </div>

          <div class="proof-card">
            <h3>Technical Sources</h3>
            <p>The source layer: the six formal papers, the separate alignment paper, and protected application directions.</p>
          </div>

          <div class="proof-card">
            <h3>Downloads</h3>
            <p>Bundled review bodies designed for deeper reading and AI-assisted inspection in larger continuous context.</p>
          </div>
        </div>

        <p class="micro-punch">
          The work can be read,
          challenged,
          and independently reviewed.
        </p>

        <div class="link-list">
          <a href="/en/theory/">Go to Theory →</a>
          <a href="/en/papers/">Go to Technical Sources →</a>
          <a href="/en/downloads/">Go to Downloads →</a>
        </div>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card">
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
    <div class="section-card">
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
