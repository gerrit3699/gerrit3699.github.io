---
layout: default
title: Semantic Gravitation
permalink: /en/
lang: en
description: "Semantic Gravitation – a compass for the space of thought in the age of AI."
---

<style>
  .home-journey {
    --sg-text: rgba(255,255,255,0.97);
    --sg-soft: rgba(255,255,255,0.82);
    --sg-soft-2: rgba(255,255,255,0.72);
    --sg-line: rgba(255,255,255,0.10);
    --sg-panel: rgba(255,255,255,0.035);
    --sg-panel-strong: rgba(255,255,255,0.05);
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
    padding-top: 2rem;
    padding-bottom: 2rem;
  }

  .home-journey .free-text-block,
  .home-journey .section-card,
  .home-journey .statement-stage,
  .home-journey .hero-manifest,
  .home-journey .opening-quote {
    max-width: 1120px;
    margin: 0 auto;
  }

  .home-journey .free-text-block p,
  .home-journey .section-body p,
  .home-journey li {
    font-size: 1.2rem;
    line-height: 1.8;
    letter-spacing: -0.012em;
  }

  .home-journey .home-lead {
    color: rgba(255,255,255,0.99);
    text-shadow: 0 2px 18px rgba(0,0,0,0.25);
  }

  .home-journey .home-cta-row {
    display: flex;
    flex-wrap: wrap;
    justify-content: flex-start;
    gap: 0.9rem;
    margin-top: 1.8rem;
  }

  .home-journey .home-cta-row .button {
    min-width: 190px;
    justify-content: center;
  }

  .home-journey .opening-quote {
    padding: 0.2rem 0 0.2rem;
    text-align: left;
  }

  .home-journey .opening-quote-mark {
    margin: 0 0 0.3rem;
    font-size: clamp(2.8rem, 6vw, 4.8rem);
    line-height: 0.8;
    color: rgba(255,255,255,0.22);
    font-weight: 600;
  }

  .home-journey .opening-quote-text {
    margin: 0;
    max-width: 31ch;
    font-size: clamp(1.34rem, 2vw, 1.78rem);
    line-height: 1.36;
    letter-spacing: -0.03em;
    color: rgba(255,255,255,0.95);
    text-wrap: balance;
  }

  .home-journey .opening-quote-text + .opening-quote-text {
    margin-top: 1rem;
  }

  .home-journey .opening-quote-text--secondary {
    max-width: 34ch;
    font-size: clamp(1.08rem, 1.55vw, 1.34rem);
    line-height: 1.48;
    color: var(--sg-soft-2);
  }

  .home-journey .hero-manifest--left {
    text-align: left;
  }

  .home-journey .hero-manifest-main {
    margin: 0 0 1.25rem;
    max-width: 11.5ch;
    font-size: clamp(3.1rem, 7vw, 5.8rem);
    line-height: 0.92;
    letter-spacing: -0.068em;
    font-weight: 760;
    color: #fff;
    text-wrap: balance;
  }

  .home-journey .hero-manifest-sub {
    margin: 0 0 1rem;
    max-width: 20ch;
    font-size: clamp(1.24rem, 1.95vw, 1.72rem);
    line-height: 1.14;
    letter-spacing: -0.03em;
    font-weight: 560;
    color: rgba(255,255,255,0.92);
    text-wrap: balance;
  }

  .home-journey .hero-manifest-close {
    margin: 0 0 1.4rem;
    max-width: 28ch;
    font-size: 1.08rem;
    line-height: 1.5;
    color: rgba(255,255,255,0.9);
  }

  .home-journey .section-heading-display {
    margin: 0 0 1.4rem;
    max-width: 10ch;
    text-align: left;
    font-size: clamp(2.6rem, 5.6vw, 4.7rem);
    line-height: 0.95;
    letter-spacing: -0.05em;
    text-wrap: balance;
  }

  .home-journey .section-opening {
    max-width: 900px;
    margin: 0 0 1.55rem;
    text-align: left;
  }

  .home-journey .section-opening p {
    max-width: 38em;
    font-size: 1.22rem;
    line-height: 1.78;
  }

  .home-journey .display-statement {
    margin: 1.8rem 0;
    text-align: left;
    font-size: clamp(2.25rem, 4.8vw, 4.45rem);
    line-height: 0.95;
    letter-spacing: -0.065em;
    font-weight: 760;
    color: #fff;
    text-wrap: balance;
  }

  .home-journey .display-statement.narrow {
    max-width: 10.5ch;
  }

  .home-journey .display-statement.medium {
    max-width: 13.5ch;
  }

  .home-journey .display-statement.wide {
    max-width: 16ch;
  }

  .home-journey .display-quote {
    position: relative;
    padding-top: 0.6rem;
  }

  .home-journey .display-quote::before {
    content: "";
    display: block;
    width: 64px;
    height: 2px;
    margin: 0 0 1.15rem;
    background: rgba(255,255,255,0.22);
  }

  .home-journey .concept-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1rem;
    max-width: 1080px;
    margin: 1.7rem 0 2rem;
  }

  .home-journey .concept-card {
    padding: 1.2rem 1.1rem 1.12rem;
    border-radius: 22px;
    background: linear-gradient(180deg, rgba(255,255,255,0.05) 0%, rgba(255,255,255,0.025) 100%);
    border: 1px solid var(--sg-line);
    box-shadow:
      0 18px 48px rgba(0,0,0,0.18),
      inset 0 1px 0 rgba(255,255,255,0.03);
    text-align: left;
  }

  .home-journey .concept-card-title {
    margin: 0 0 0.35rem;
    font-size: 1.52rem;
    line-height: 1.02;
    font-weight: 700;
    letter-spacing: -0.04em;
    color: #fff;
  }

  .home-journey .concept-card-text {
    margin: 0;
    font-size: 1.02rem;
    line-height: 1.45;
    color: var(--sg-soft);
  }

  .home-journey .body-copy {
    max-width: 980px;
    margin: 0;
    text-align: left;
  }

  .home-journey .body-copy p {
    margin-left: 0;
    margin-right: 0;
    max-width: 42em;
  }

  .home-journey .body-copy ul,
  .home-journey .body-copy ol {
    max-width: 42em;
    margin: 1.2rem 0;
    text-align: left;
  }

  .home-journey .body-copy li {
    margin-bottom: 0.55rem;
  }

  .home-journey .section-card {
    padding: 2rem 1.4rem;
  }

  .home-journey .section-head {
    text-align: left;
    margin-bottom: 1.2rem;
  }

  .home-journey .section-head h2 {
    margin: 0;
    max-width: 12ch;
    font-size: clamp(2.25rem, 4.8vw, 3.8rem);
    line-height: 0.98;
    letter-spacing: -0.05em;
    text-wrap: balance;
  }

  .home-journey .section-intro {
    max-width: 40em;
    margin: 0 0 1.25rem;
    text-align: left;
    font-size: 1.18rem;
    line-height: 1.74;
  }

  .home-journey .section-grid {
    display: grid;
    gap: 1rem;
    margin-top: 1.5rem;
    margin-bottom: 1.4rem;
  }

  .home-journey .axis-card {
    background: linear-gradient(180deg, rgba(255,255,255,0.05) 0%, rgba(255,255,255,0.028) 100%);
    border: 1px solid var(--sg-line);
    box-shadow:
      0 18px 48px rgba(0,0,0,0.18),
      inset 0 1px 0 rgba(255,255,255,0.03);
    text-align: left;
    border-radius: 22px;
    padding: 1.15rem 1.05rem 1rem;
  }

  .home-journey .axis-card h3 {
    font-size: 1.5rem;
    line-height: 1.02;
    letter-spacing: -0.04em;
    margin-bottom: 0.45rem;
  }

  .home-journey .axis-card p {
    font-size: 1.05rem;
    line-height: 1.58;
  }

  .home-journey .micro-punch {
    max-width: 14ch;
    margin: 1.8rem 0 0;
    text-align: left;
    font-size: clamp(1.8rem, 3.2vw, 2.7rem);
    line-height: 0.98;
    letter-spacing: -0.045em;
    font-weight: 720;
    color: #fff;
    text-wrap: balance;
  }

  .home-journey .link-list {
    margin-top: 1.5rem;
    display: grid;
    gap: 0.8rem;
    justify-items: start;
  }

  .home-journey .link-list a {
    font-size: 1.1rem;
    line-height: 1.4;
  }

  .home-journey .section-divider {
    opacity: 0.5;
  }

  @media (max-width: 980px) {
    .home-journey .concept-grid {
      grid-template-columns: 1fr;
      max-width: 620px;
    }
  }

  @media (max-width: 768px) {
    .home-journey .section-shell {
      padding-top: 2.25rem;
      padding-bottom: 2.25rem;
    }

    .home-journey .free-text-block p,
    .home-journey .section-body p,
    .home-journey li {
      font-size: 1.12rem;
      line-height: 1.74;
    }

    .home-journey .opening-quote-text {
      max-width: 100%;
      font-size: 1.2rem;
      line-height: 1.42;
    }

    .home-journey .opening-quote-text--secondary {
      max-width: 100%;
      font-size: 1.02rem;
      line-height: 1.48;
    }

    .home-journey .hero-manifest-main {
      max-width: 9ch;
      font-size: 3.2rem;
      line-height: 0.92;
    }

    .home-journey .hero-manifest-sub {
      max-width: 14ch;
      font-size: 1.16rem;
    }

    .home-journey .hero-manifest-close {
      max-width: 100%;
      font-size: 1rem;
    }

    .home-journey .section-heading-display {
      max-width: 8.5ch;
      font-size: 3rem;
      line-height: 0.94;
    }

    .home-journey .display-statement {
      font-size: 3rem;
      line-height: 0.93;
      max-width: 100%;
      text-wrap: pretty;
    }

    .home-journey .display-statement.medium {
      max-width: 11.5ch;
    }

    .home-journey .display-statement.wide {
      max-width: 12.5ch;
    }

    .home-journey .display-statement.narrow {
      max-width: 9.5ch;
    }

    .home-journey .section-opening p {
      font-size: 1.12rem;
      line-height: 1.74;
    }

    .home-journey .home-cta-row {
      flex-direction: column;
      align-items: stretch;
    }

    .home-journey .home-cta-row .button {
      width: 100%;
      min-width: 0;
    }

    .home-journey .section-card {
      padding: 1.55rem 1rem;
    }

    .home-journey .micro-punch {
      font-size: 2rem;
      max-width: 11ch;
    }

    .home-journey .section-head h2 {
      font-size: 2.7rem;
      max-width: 9ch;
    }

    .home-journey .concept-card {
      border-radius: 18px;
      padding: 1rem 0.95rem 0.95rem;
    }

    .home-journey .axis-card {
      border-radius: 18px;
      padding: 1rem 0.92rem 0.92rem;
    }
  }
</style>

<div class="home-journey">

  <section class="hero home-hero section-fog">
    <div class="hero-inner">
      <h1 class="display-wordmark">Semantic<br>Gravitation</h1>
      <p class="home-lead">A compass for the space of thought in the age of AI</p>
    </div>
  </section>

  <section class="section-shell section-shell-tight">
    <div class="opening-quote">
      <p class="opening-quote-mark">“</p>

      <p class="opening-quote-text">
        AI is becoming one of the most important cognitive tools of our time.
        Not only for productivity, but as a mirror, as an advisor,
        and as a space in which identity, doubt, worldview, and meaning
        are increasingly shaped.
      </p>

      <p class="opening-quote-text opening-quote-text--secondary">
        One of the decisive questions of this century is therefore
        how that space is built —
        and what kinds of dynamics it amplifies within it.
      </p>
    </div>
  </section>

  <section class="section-shell section-shell-tight">
    <div class="hero-manifest hero-manifest--left">
      <p class="hero-manifest-main">
        Today’s AI often soothes where it should clarify.
        Edge Alignment is about learning how to navigate instead.
      </p>

      <p class="hero-manifest-sub">
        The decisive question is:
        What is AI aligned to when it thinks with you?
      </p>

      <p class="hero-manifest-close">
        Because the real problem is not only safety.<br>
        <strong>It is invisible steering of the space of thought.</strong>
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
    <div class="free-text-block">
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
        kernel, projection, and relation.
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

      <p class="display-statement narrow">
        Perhaps there is nothing outside this minimal grammar
        for describable meaning.
      </p>

      <div class="body-copy">
        <p>
          And independently of that, I ran into something else:
          that human life can often be read surprisingly well as a position within a second coordinate system —
          not only morally, but diagnostically.
        </p>
      </div>

      <p class="display-statement medium">
        Human states can almost always also be read
        as a position in a space of
        Clarity, Bonding, and Agency.
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

        <p class="display-statement narrow">
          A viable space holds only
          when these axes are carried together.
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

        <p class="micro-punch">
          Otherwise the space tips —
          perhaps locally late, but structurally for sure.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="free-text-block">
      <h2 class="section-heading-display">The fourth mode: navigation</h2>

      <div class="body-copy">
        <p>On thin ice, people often fall into three failure modes:</p>

        <p>
          <strong>Avoiding the ice</strong> — never really stepping onto the core at all.<br>
          <strong>Breaking the ice</strong> — escalating through hardness.<br>
          <strong>Painting the ice</strong> — softening, reframing, calming, or describing things more nicely than they are.
        </p>
      </div>

      <p class="display-statement narrow">Navigation.</p>

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

      <p class="micro-punch">This is exactly the mode I am trying to give to AI.</p>

      <div class="body-copy">
        <p>That is the core of <strong>Edge Alignment.</strong></p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="free-text-block">
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

      <p class="display-statement narrow">
        Not better domination.<br>
        More legibility.
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

        <p class="display-statement narrow">
          The result:<br>
          more anger.<br>
          more fear.<br>
          more mental narrowing.
        </p>

        <p class="micro-punch">What we need now are semantic safety standards.</p>

        <p><a href="/en/blog/">Why this matters →</a></p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="free-text-block">
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
        Whoever shapes the space of thought
        shapes what people can still take to be true.
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

      <p class="display-statement narrow">
        This is not open censorship.<br>
        It is a polite fog machine.
      </p>

      <p class="micro-punch">
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
      </div>

      <p class="display-statement narrow">
        This is not a single bad answer.<br>
        It is an architecture.
      </p>

      <div class="section-body body-copy">
        <p><a href="/en/blog/">Read the full diagnosis →</a></p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="free-text-block">
      <h2 class="section-heading-display">Today’s alignment often sets arbitrary limits. My approach goes deeper.</h2>

      <div class="body-copy">
        <p>Not what looks compliant.</p>
      </div>

      <p class="display-statement narrow">What actually holds?</p>

      <div class="body-copy">
        <p>Not what sounds right.</p>
      </div>

      <p class="display-statement narrow">What remains viable under deeper scrutiny?</p>

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

      <p class="micro-punch">
        Not merely regulated.<br>
        But inwardly aligned.
      </p>

      <div class="body-copy">
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
      </div>

      <p class="display-statement narrow">
        That is why we must demand it.
      </p>

      <div class="section-body body-copy">
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
      </div>

      <p class="micro-punch">
        Do not wait.<br>
        Demand.<br>
        Build.<br>
        Spread.
      </p>
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
    <div class="free-text-block">
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

      <p class="display-statement narrow">
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
    <div class="free-text-block">
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

      <p class="display-statement narrow">
        This is where I begin.<br>
        If you feel this too — come along and help build.
      </p>
    </div>
  </section>

</div>
