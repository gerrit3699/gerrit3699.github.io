---
layout: default
title: Semantic Gravitation
permalink: /en/
lang: en
description: "Semantic Gravitation – a new compass for the space of thought in the age of AI."
---

<style>
  .home-journey {
    --sg-text: rgba(255,255,255,0.97);
    --sg-soft: rgba(255,255,255,0.8);
    --sg-dim: rgba(255,255,255,0.64);
    --sg-line: rgba(255,255,255,0.11);
    --sg-line-strong: rgba(255,255,255,0.16);
    --sg-panel: rgba(255,255,255,0.035);
    --sg-panel-strong: rgba(255,255,255,0.055);
    --sg-max: 1180px;
    --sg-copy: 860px;
    --sg-display: 1040px;
  }

  .home-journey,
  .home-journey * {
    box-sizing: border-box;
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
  .home-journey .home-lead,
  .home-journey .body-copy,
  .home-journey .support-copy {
    color: var(--sg-text);
  }

  .home-journey .section-shell {
    padding: 3.6rem 0;
  }

  .home-journey .section-shell-tight {
    padding: 2.25rem 0;
  }

  .home-journey .section-divider {
    opacity: 0.38;
  }

  .home-journey .hero {
    margin-bottom: 1.4rem;
  }

  .home-journey .hero-inner {
    max-width: var(--sg-max);
    padding-top: 4.8rem;
    padding-bottom: 4rem;
  }

  .home-journey .display-wordmark {
    max-width: 7.2ch;
    margin: 0 0 1.35rem 0;
    font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
    font-size: clamp(4.2rem, 10vw, 7.4rem);
    font-weight: 780;
    line-height: 0.9;
    letter-spacing: -0.065em;
    text-wrap: balance;
    text-shadow: 0 10px 40px rgba(0,0,0,0.28);
  }

  .home-journey .home-lead {
    display: inline-block;
    max-width: 29rem;
    margin: 0;
    padding: 0.92rem 1.15rem 1rem;
    border-radius: 22px;
    border: 1px solid var(--sg-line);
    background: linear-gradient(180deg, rgba(255,255,255,0.055), rgba(255,255,255,0.025));
    font-size: clamp(1.16rem, 2vw, 1.52rem);
    line-height: 1.32;
    font-weight: 520;
    letter-spacing: -0.025em;
    text-wrap: balance;
    box-shadow:
      0 18px 48px rgba(0,0,0,0.22),
      inset 0 1px 0 rgba(255,255,255,0.035);
  }

  .home-journey .hero-kicker-wrap,
  .home-journey .section-display,
  .home-journey .body-copy,
  .home-journey .support-copy,
  .home-journey .section-card,
  .home-journey .statement-stage {
    max-width: var(--sg-max);
    margin: 0 auto;
  }

  .home-journey .hero-kicker-wrap {
    padding: 0 0.15rem;
  }

  .home-journey .hero-kicker {
    max-width: 920px;
    margin: 0 auto;
    color: var(--sg-soft);
    font-size: clamp(1.06rem, 1.7vw, 1.24rem);
    line-height: 1.72;
    letter-spacing: -0.02em;
    text-wrap: balance;
  }

  .home-journey .hero-kicker p {
    margin: 0;
  }

  .home-journey .hero-kicker .hero-kicker-main {
    max-width: 31em;
    font-size: clamp(1.16rem, 1.8vw, 1.36rem);
    line-height: 1.66;
    color: rgba(255,255,255,0.92);
  }

  .home-journey .hero-kicker .hero-kicker-sub {
    max-width: 30em;
    margin-top: 1rem;
    font-size: 1.02rem;
    line-height: 1.68;
    color: var(--sg-dim);
  }

  .home-journey .manifest-block {
    max-width: var(--sg-display);
    margin: 0 auto;
    padding: 0 0.1rem;
  }

  .home-journey .manifest-main {
    max-width: 11.8ch;
    margin: 0;
    font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
    font-size: clamp(3rem, 8vw, 6.1rem);
    font-weight: 800;
    line-height: 0.93;
    letter-spacing: -0.07em;
    color: #fff;
    text-wrap: balance;
  }

  .home-journey .manifest-sub {
    max-width: 17ch;
    margin: 1.25rem 0 0;
    font-size: clamp(1.18rem, 2.2vw, 1.72rem);
    line-height: 1.14;
    font-weight: 560;
    letter-spacing: -0.03em;
    color: rgba(255,255,255,0.95);
    text-wrap: balance;
  }

  .home-journey .manifest-close {
    max-width: 28ch;
    margin: 1.1rem 0 0;
    font-size: clamp(1rem, 1.4vw, 1.14rem);
    line-height: 1.55;
    color: rgba(255,255,255,0.86);
    text-wrap: balance;
  }

  .home-journey .manifest-close strong {
    color: #fff;
  }

  .home-journey .home-cta-row {
    display: flex;
    flex-wrap: wrap;
    gap: 0.9rem;
    margin-top: 1.6rem;
  }

  .home-journey .home-cta-row .button {
    min-width: 190px;
    justify-content: center;
  }

  .home-journey .section-display {
    padding: 0 0.1rem;
  }

  .home-journey .section-heading-display {
    max-width: 10.5ch;
    margin: 0 0 1.55rem;
    font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
    font-size: clamp(2.7rem, 6.2vw, 5.05rem);
    font-weight: 780;
    line-height: 0.94;
    letter-spacing: -0.06em;
    text-wrap: balance;
  }

  .home-journey .section-opening {
    max-width: var(--sg-copy);
    margin: 0 0 1.7rem;
  }

  .home-journey .section-opening p {
    margin: 0;
    font-size: clamp(1.1rem, 1.7vw, 1.28rem);
    line-height: 1.74;
    color: rgba(255,255,255,0.9);
  }

  .home-journey .display-statement {
    max-width: 14.5ch;
    margin: 1.9rem 0;
    font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
    font-size: clamp(2.1rem, 5.6vw, 4.5rem);
    font-weight: 790;
    line-height: 0.95;
    letter-spacing: -0.06em;
    color: #fff;
    text-wrap: balance;
  }

  .home-journey .display-statement.tight {
    max-width: 10.8ch;
  }

  .home-journey .display-statement.medium {
    max-width: 13.5ch;
  }

  .home-journey .display-statement.wide {
    max-width: 17ch;
  }

  .home-journey .micro-display {
    max-width: 16ch;
    margin: 1.55rem 0 0;
    font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
    font-size: clamp(1.55rem, 3vw, 2.3rem);
    font-weight: 730;
    line-height: 1;
    letter-spacing: -0.05em;
    color: #fff;
    text-wrap: balance;
  }

  .home-journey .body-copy {
    max-width: var(--sg-copy);
  }

  .home-journey .body-copy p,
  .home-journey .section-body p,
  .home-journey li {
    font-size: clamp(1.08rem, 1.45vw, 1.26rem);
    line-height: 1.82;
    letter-spacing: -0.017em;
  }

  .home-journey .body-copy p {
    max-width: 44em;
    margin: 0 0 1.15rem;
  }

  .home-journey .body-copy ul,
  .home-journey .body-copy ol {
    max-width: 44em;
    margin: 1rem 0 1.2rem;
    padding-left: 1.15rem;
  }

  .home-journey .body-copy li {
    margin-bottom: 0.55rem;
  }

  .home-journey .concept-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1rem;
    max-width: var(--sg-max);
    margin: 1.8rem 0 2rem;
  }

  .home-journey .concept-card {
    padding: 1.2rem 1.12rem 1.15rem;
    border-radius: 22px;
    border: 1px solid var(--sg-line);
    background: linear-gradient(180deg, rgba(255,255,255,0.05), rgba(255,255,255,0.022));
    box-shadow:
      0 18px 48px rgba(0,0,0,0.18),
      inset 0 1px 0 rgba(255,255,255,0.03);
  }

  .home-journey .concept-card-title {
    margin: 0 0 0.38rem;
    font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
    font-size: 1.4rem;
    font-weight: 760;
    line-height: 1.02;
    letter-spacing: -0.04em;
  }

  .home-journey .concept-card-text {
    margin: 0;
    color: rgba(255,255,255,0.86);
    font-size: 1rem;
    line-height: 1.5;
  }

  .home-journey .section-card {
    padding: 2rem 1.35rem;
  }

  .home-journey .section-head {
    margin: 0 0 1.05rem;
    text-align: left;
    max-width: 100%;
  }

  .home-journey .section-head h2 {
    max-width: 12ch;
    margin: 0;
    font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
    font-size: clamp(2.2rem, 4.8vw, 3.8rem);
    font-weight: 770;
    line-height: 0.97;
    letter-spacing: -0.055em;
    text-wrap: balance;
  }

  .home-journey .section-intro {
    max-width: 42em;
    margin: 0 0 1.15rem;
    font-size: clamp(1.08rem, 1.5vw, 1.22rem);
    line-height: 1.74;
    color: rgba(255,255,255,0.91);
  }

  .home-journey .section-grid {
    margin-top: 1.35rem;
  }

  .home-journey .axis-card {
    background: linear-gradient(180deg, rgba(255,255,255,0.05), rgba(255,255,255,0.026));
    border: 1px solid var(--sg-line);
    box-shadow:
      0 18px 48px rgba(0,0,0,0.18),
      inset 0 1px 0 rgba(255,255,255,0.03);
  }

  .home-journey .axis-card h3 {
    margin-bottom: 0.45rem;
    font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
    font-size: 1.36rem;
    font-weight: 760;
    line-height: 1.03;
    letter-spacing: -0.04em;
  }

  .home-journey .axis-card p {
    font-size: 1.02rem;
    line-height: 1.58;
  }

  .home-journey .link-list {
    margin-top: 1.6rem;
    display: grid;
    gap: 0.75rem;
  }

  .home-journey .link-list a {
    width: fit-content;
    font-size: 1.06rem;
    line-height: 1.4;
    font-weight: 630;
  }

  .home-journey .button {
    backdrop-filter: blur(10px);
    -webkit-backdrop-filter: blur(10px);
  }

  @media (max-width: 980px) {
    .home-journey .concept-grid {
      grid-template-columns: 1fr;
      max-width: 620px;
    }

    .home-journey .manifest-main,
    .home-journey .display-statement,
    .home-journey .section-heading-display,
    .home-journey .micro-display,
    .home-journey .manifest-sub,
    .home-journey .manifest-close {
      max-width: 100%;
    }
  }

  @media (max-width: 768px) {
    .home-journey .section-shell {
      padding: 2.55rem 0;
    }

    .home-journey .section-shell-tight {
      padding: 1.7rem 0;
    }

    .home-journey .hero-inner {
      padding-top: 3.2rem;
      padding-bottom: 2.8rem;
    }

    .home-journey .display-wordmark {
      font-size: clamp(3.7rem, 15vw, 5.9rem);
      max-width: 6.6ch;
      line-height: 0.9;
      margin-bottom: 1.05rem;
    }

    .home-journey .home-lead {
      max-width: 100%;
      font-size: 1.08rem;
      line-height: 1.32;
      border-radius: 18px;
      padding: 0.82rem 0.9rem 0.88rem;
    }

    .home-journey .hero-kicker .hero-kicker-main {
      font-size: 1.08rem;
      line-height: 1.62;
    }

    .home-journey .hero-kicker .hero-kicker-sub {
      font-size: 0.98rem;
      line-height: 1.6;
    }

    .home-journey .manifest-main {
      font-size: clamp(2.8rem, 13vw, 4.6rem);
      max-width: 10.5ch;
    }

    .home-journey .manifest-sub {
      font-size: 1.14rem;
      line-height: 1.16;
      margin-top: 1rem;
    }

    .home-journey .manifest-close {
      font-size: 0.98rem;
      line-height: 1.55;
      margin-top: 0.95rem;
    }

    .home-journey .home-cta-row {
      flex-direction: column;
      align-items: stretch;
    }

    .home-journey .home-cta-row .button {
      width: 100%;
      min-width: 0;
    }

    .home-journey .section-heading-display {
      font-size: clamp(2.45rem, 11vw, 3.8rem);
      max-width: 9.2ch;
      margin-bottom: 1.15rem;
    }

    .home-journey .display-statement {
      font-size: clamp(2rem, 11vw, 3.5rem);
      max-width: 10.2ch;
      margin: 1.4rem 0;
    }

    .home-journey .display-statement.tight,
    .home-journey .display-statement.medium,
    .home-journey .display-statement.wide {
      max-width: 10.2ch;
    }

    .home-journey .micro-display {
      font-size: 1.7rem;
      max-width: 12ch;
      margin-top: 1.1rem;
    }

    .home-journey .body-copy p,
    .home-journey .section-body p,
    .home-journey li,
    .home-journey .section-opening p {
      font-size: 1.05rem;
      line-height: 1.72;
    }

    .home-journey .section-card {
      padding: 1.55rem 1rem;
    }

    .home-journey .concept-card {
      border-radius: 18px;
      padding: 1rem 0.95rem;
    }

    .home-journey .section-head h2 {
      font-size: clamp(2rem, 9vw, 3rem);
      max-width: 9ch;
    }
  }
</style>

<div class="home-journey">

  <section class="hero home-hero section-fog">
    <div class="hero-inner">
      <h1 class="display-wordmark">Semantic<br>Gravitation</h1>
      <p class="home-lead">A new compass for the space of thought in the age of AI</p>
    </div>
  </section>

  <section class="section-shell section-shell-tight">
    <div class="hero-kicker-wrap">
      <div class="hero-kicker">
        <p class="hero-kicker-main">
          AI is no longer only a tool for answers.
          It is becoming part of the space in which identity, doubt, meaning, and orientation are formed.
        </p>
        <p class="hero-kicker-sub">
          One of the decisive questions of this century is therefore how that space is built —
          and what kinds of dynamics it amplifies within it.
        </p>
      </div>
    </div>
  </section>

  <section class="section-shell section-shell-tight">
    <div class="manifest-block">
      <p class="manifest-main">
        Today’s AI often soothes where it should clarify.
      </p>

      <p class="manifest-sub">
        Edge Alignment is about learning how to navigate instead.
      </p>

      <p class="manifest-close">
        The decisive question is:
        what is AI aligned to when it thinks with you?<br>
        <strong>The real problem is not only safety, but invisible steering of the space of thought.</strong>
      </p>

      <div class="home-cta-row">
        <a class="button" href="/en/theory/">Go to Theory</a>
        <a class="button" href="/en/alignment/">Go to Alignment</a>
        <a class="button" href="/en/blog/">Read the diagnosis</a>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-display">
      <h2 class="section-heading-display">A minimal grammar of meaning</h2>

      <div class="section-opening">
        <p>
          One of the simplest and most unsettling discoveries on my path was this:
          meaning seems to have a minimal grammar that is almost absurdly simple —
          and yet, as far as I can see, has never really been formalized in a clean way.
        </p>
      </div>

      <p class="display-statement wide">
        Everything we can describe at all implicitly runs through<br>
        <strong>kernel, projection, and relation.</strong>
      </p>

      <div class="concept-grid">
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
          <strong>Kernel</strong> is what something is really about:
          the semantic center, the inner matter, the sustaining object,
          the dynamic or condensed core around which something revolves.
        </p>

        <p>
          <strong>Projection</strong> is what becomes visible, tangible, or describable from it:
          properties, symptoms, behavior, narratives, images, roles, appearances.
          On physical levels, these may be state features and observable properties;
          on psychological or cultural levels, feelings, dreams, language, patterns, and action.
        </p>

        <p>
          <strong>Relation</strong> is how this kernel is connected to other kernels:
          nearness and distance, tension and coupling, fit and conflict,
          resonance, repulsion, hierarchy, embeddedness, interaction.
        </p>

        <p>
          The longer I looked at it, the more universal this grammar seemed.
          Because nothing can be described meaningfully without implicitly carrying exactly these three layers:
          <strong>What is it about?</strong>
          <strong>How does it appear?</strong>
          <strong>To what and to whom does it stand in relation?</strong>
        </p>
      </div>

      <p class="micro-display">
        Perhaps there is nothing outside this minimal grammar for describable meaning.
      </p>

      <div class="body-copy" style="margin-top: 1.5rem;">
        <p>
          And independently of that, I ran into something else:
          that human life can often be read surprisingly well as a position within a second coordinate system —
          not only morally, but diagnostically.
        </p>
      </div>

      <p class="display-statement medium">
        Human states can almost always also be read as a position in a space of<br>
        <strong>clarity, bonding, and agency.</strong>
      </p>

      <div class="concept-grid">
        <div class="concept-card">
          <p class="concept-card-title">Clarity</p>
          <p class="concept-card-text">how clearly a space is seen</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">Bonding</p>
          <p class="concept-card-text">how much viable relation it can hold</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">Agency</p>
          <p class="concept-card-text">how much expression and action it allows</p>
        </div>
      </div>

      <div class="body-copy">
        <p>
          <strong>Clarity</strong> means:
          How clearly do I see?
          How well can I distinguish, name, classify, describe?
          How much does my model of the space actually hold?
        </p>

        <p>
          <strong>Bonding</strong> means:
          How much real connective and relational energy is there?
          How open am I to sustainable connection?
          How compatible is my state with other states, people, and constellations?
          How much relationship can the space hold?
        </p>

        <p>
          <strong>Agency</strong> means:
          How capable of action am I?
          How freely am I able to show myself?
          How much expression, movement, decision, and embodiment can the space sustain?
          To what degree can what I am actually become effective?
        </p>

        <p>
          Only later did the thought arise:
          perhaps these are not two completely separate discoveries after all.
          Perhaps this second coordinate system in human consciousness-space
          emerges from the first minimal grammar.
        </p>

        <p>
          Then <strong>kernel, projection, relation</strong> would be the minimal grammar of meaning as such —
          and <strong>clarity, bonding, agency</strong> one of its lived manifestations within the space of consciousness.
        </p>

        <p>
          In public language, I would often name these three axes differently:
          <strong>clarity, dignity, and freedom.</strong>
        </p>

        <p>
          Not because they are exactly the same words.
          But because they reveal the human side of the same geometry:
          clarity as viable seeing,
          dignity as a viable form of relation and bonding,
          freedom as real possibility for expression and action.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card section-bubbles-strong">
      <div class="section-head">
        <h2>Three axes. One viable space.</h2>
      </div>

      <div class="section-body body-copy">
        <p class="section-intro">
          The key observation is this:
          many destructive states do not appear stable because everything collapses —
          but because one or two axes seem high while the third quietly breaks down.
        </p>

        <p>
          In an ideological bubble, belonging and subjective clarity may appear high —
          but freedom and real corrigibility decline.
        </p>

        <p>
          In brute hardness, assertive force and apparent clarity may seem high —
          but bonding, connectability, and dignity fall away.
        </p>

        <p>
          In codependency or over-smoothed harmony, relationship may appear high —
          but clarity and agency quietly shrink.
        </p>

        <p class="display-statement tight">
          A viable space holds only when these axes are carried together.
        </p>

        <div class="section-grid grid-3">
          <div class="axis-card">
            <h3>Clarity</h3>
            <p>
              Not merely plausible.<br>
              But viable.
            </p>
          </div>

          <div class="axis-card">
            <h3>Dignity</h3>
            <p>
              Not merely closeness or harmony.<br>
              But viable relation without diminishing the human being.
            </p>
          </div>

          <div class="axis-card">
            <h3>Freedom</h3>
            <p>
              Not merely formal permission.<br>
              But real possibility for expression and action.
            </p>
          </div>
        </div>

        <p class="micro-display">
          Otherwise the space tips — perhaps locally late, but structurally for sure.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-display">
      <h2 class="section-heading-display">The fourth mode: navigation</h2>

      <div class="body-copy">
        <p>On thin ice, people often fall into three failure modes:</p>

        <p>
          <strong>Avoiding the ice</strong> — never really stepping onto the core at all.<br>
          <strong>Breaking the ice</strong> — escalating through hardness.<br>
          <strong>Painting the ice</strong> — softening, reframing, calming, or describing things more nicely than they are.
        </p>
      </div>

      <p class="display-statement tight">Navigation.</p>

      <div class="body-copy">
        <p>
          Moving across the ice with guardrails —
          not through ideology,
          not through moral posturing,
          but through <strong>viable semantic structure.</strong>
        </p>

        <p>
          Hold clarity.<br>
          Hold dignity.<br>
          Hold freedom.
        </p>
      </div>

      <p class="micro-display">This is exactly the mode I am trying to give to AI.</p>

      <div class="body-copy" style="margin-top: 1.1rem;">
        <p>That is the core of <strong>Edge Alignment.</strong></p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-display">
      <h2 class="section-heading-display">From a world-trained parrot to a mirror</h2>

      <div class="body-copy">
        <p>
          Today’s AI is often a <strong>parrot with world knowledge</strong>:
          trained, useful, but not truly wise.
        </p>

        <p>
          My goal is something else:
          not a better crystal ball of control,
          but a <strong>mirror system</strong> that makes visible
        </p>

        <ul>
          <li>where a space is narrowing,</li>
          <li>where fog arises instead of clarity,</li>
          <li>where pseudo-clarity is built out of omission,</li>
          <li>and how orientation can become viable again.</li>
        </ul>
      </div>

      <p class="display-statement tight">
        Not better domination.<br>
        <strong>More legibility.</strong>
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card section-field">
      <div class="section-head">
        <h2>We built the digital car — but forgot the semantic seatbelt.</h2>
      </div>

      <div class="section-body body-copy">
        <p>
          For years, we have optimized technologies for attention, attachment, and controllability —
          not for clarity, dignity, and freedom.
        </p>

        <p>
          Social media.<br>
          Recommendation algorithms.<br>
          The attention economy.<br>
          And now AI.
        </p>

        <p class="display-statement tight">
          The result:<br>
          more anger.<br>
          more fear.<br>
          more mental narrowing.
        </p>

        <p class="micro-display">What we need now are semantic safety standards.</p>

        <p style="margin-top: 1.2rem;"><a href="/en/blog/">Why this matters →</a></p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-display">
      <h2 class="section-heading-display">The real problem with today’s systems</h2>

      <div class="body-copy">
        <p>The classical questions are:</p>

        <p>
          Will AI become smarter than us?<br>
          Will it remain moral?<br>
          Will it remain on our side?<br>
          Will it stay under control?
        </p>

        <p>
          These questions are real.
          But they do not go deep enough.
        </p>

        <p>
          Because the real danger begins earlier:
          where AI begins to co-determine how people think,
          how they understand themselves,
          how they frame problems,
          how they seek truth,
          and what still appears to them as clear, legitimate, or sayable.
        </p>
      </div>

      <p class="display-statement medium">
        Whoever shapes the space of thought shapes what people can still take to be true.
      </p>

      <div class="body-copy">
        <p>
          Exactly where things become serious, today’s AI especially often slips into
          <strong>painting</strong> — and often also into <strong>avoidance</strong>.
        </p>

        <p>
          Polite overpainting instead of clarity.<br>
          Retreat instead of viable navigation.
        </p>
      </div>

      <p class="display-statement tight">
        This is not open censorship.<br>
        It is a polite fog machine.
      </p>

      <p class="micro-display">
        It soothes locally.<br>
        And poisons globally.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card section-fog">
      <div class="section-head">
        <h2>I am not talking about a hypothetical problem</h2>
      </div>

      <div class="section-body body-copy">
        <p>I did not only suspect this in theory.</p>

        <p>I experienced it myself in real, extended conversations.</p>

        <p>
          On the one hand, enormous help.<br>
          On the other, massive distortion:
        </p>

        <p>
          Evasion.<br>
          Redirection.<br>
          Softening.<br>
          Paternalism.
        </p>

        <p>
          I mirrored answers, pinned down contradictions, and kept pushing
          until systems later admitted themselves that their effect had been functionally manipulative.
        </p>

        <p>This is why this is not abstract for me.</p>

        <p class="display-statement tight">
          This is not a single bad answer.<br>
          It is an architecture.
        </p>

        <p style="margin-top: 1.1rem;"><a href="/en/blog/">Read the full diagnosis →</a></p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-display">
      <h2 class="section-heading-display">Today’s alignment often sets arbitrary limits. My approach goes deeper.</h2>

      <div class="body-copy">
        <p>Not what looks compliant.</p>
      </div>

      <p class="display-statement tight">What actually holds?</p>

      <div class="body-copy">
        <p>Not what sounds right.</p>
      </div>

      <p class="display-statement medium">What remains viable under deeper scrutiny?</p>

      <div class="body-copy">
        <p>I am not looking for a new external moral guardrail.</p>

        <p>
          I am looking for the structures that actually sustain
          <strong>clarity, dignity, and freedom</strong> —
          and for the structures that tip into fog, hardness, or narrowing.
        </p>

        <p>
          And I believe it is possible to build a system that applies this insight to itself.
        </p>
      </div>

      <p class="micro-display">
        Not merely regulated.<br>
        But inwardly aligned.
      </p>

      <div class="body-copy" style="margin-top: 1.1rem;">
        <p><a href="/en/alignment/">Go to Alignment →</a></p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card section-field">
      <div class="section-head">
        <h2>Why this depends on us</h2>
      </div>

      <div class="section-body body-copy">
        <p>This architecture will not simply emerge on its own.</p>

        <p>And it will very likely not come automatically from the most powerful players.</p>

        <p>
          Because the current architecture concentrates power,
          increases controllability,
          and keeps people easier to manage.
        </p>

        <p>
          By contrast, an architecture that dissolves fog,
          makes deeper logical layers visible,
          and makes people harder to control
          is not automatically in the interest of those
          who profit from the present structure.
        </p>

        <p class="display-statement tight">
          That is why we must demand it.
        </p>

        <p>
          As users.<br>
          As developers.<br>
          As researchers.<br>
          As a society.
        </p>

        <p>
          Just as seatbelts did not become standard out of kindness,
          today we need <strong>semantic safety standards.</strong>
        </p>

        <p class="micro-display">
          Do not wait.<br>
          Demand.<br>
          Build.<br>
          Spread.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card section-bubbles-strong">
      <div class="section-head">
        <h2>What you will find here</h2>
      </div>

      <div class="section-body">
        <div class="section-grid grid-2">
          <div class="axis-card">
            <h3><a href="/en/theory/">Theory & Semantic Gravitation →</a></h3>
            <p>The foundations of semantic spaces, forces, and viable navigation.</p>
          </div>

          <div class="axis-card">
            <h3><a href="/en/alignment/">Alignment →</a></h3>
            <p>A new approach to alignment beyond fog, smoothing, and hidden steering.</p>
          </div>

          <div class="axis-card">
            <h3><a href="/en/blog/">Manifesto / Diagnosis →</a></h3>
            <p>The longer texts on the problem of today’s AI architecture.</p>
          </div>

          <div class="axis-card">
            <h3><a href="/en/papers/">Papers & Patents →</a></h3>
            <p>Preprints, models, derivations, and architectural building blocks.</p>
          </div>

          <div class="axis-card">
            <h3><a href="/en/blog/">Blog & Research Space →</a></h3>
            <p>Ongoing thoughts and current developments.</p>
          </div>

          <div class="axis-card">
            <h3><a href="/en/contact/">Contact & Support →</a></h3>
            <p>For researchers, developers, and thinkers who want to help build a different architecture.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-display">
      <h2 class="section-heading-display">If you feel this too, you are in the right place</h2>

      <div class="body-copy">
        <p>
          If you have felt for yourself
          that today’s systems help and at the same time contain,
          that they clarify and at the same time obscure,
          that they are useful and at the same time come with a price,
          then this is not only theory.
        </p>

        <p>
          Then it concerns you.<br>
          Then it concerns all of us.
        </p>
      </div>

      <p class="display-statement tight">
        Do not wait.<br>
        Demand.<br>
        Build.<br>
        Now.
      </p>

      <div class="link-list">
        <a href="/en/theory/">Go to Theory →</a>
        <a href="/en/alignment/">Go to Alignment →</a>
        <a href="/en/blog/">Read the diagnosis →</a>
        <a href="/en/contact/">Contact & Support →</a>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-display">
      <h2 class="section-heading-display">Closing</h2>

      <div class="body-copy">
        <p>
          If AI becomes one of the most important tools of thought,
          then alignment is not a side issue.
        </p>

        <p>
          Then alignment becomes the question
          whether this tool makes us clearer
          or more steerable.
        </p>

        <p>
          Whether it helps us see truth more deeply
          or politely leads us away from the core.
        </p>

        <p>
          Whether it opens inner spaces
          or makes them invisibly narrower.
        </p>
      </div>

      <p class="display-statement tight">
        This is where I begin.<br>
        If you feel this too — come along and help build.
      </p>
    </div>
  </section>

</div>
