---
layout: default
title: Semantic Gravitation
permalink: /en/
lang: en
description: "Semantic Gravitation – a compass for the space of thought in the age of AI."
---

<style>
  .home-journey .intro-copy,
  .home-journey .intro-copy p,
  .home-journey .free-text-block p,
  .home-journey .section-body p,
  .home-journey .axis-card p,
  .home-journey li,
  .home-journey .closing-line,
  .home-journey .section-intro {
    color: rgba(255,255,255,0.975);
  }

  .home-journey strong,
  .home-journey h1,
  .home-journey h2,
  .home-journey h3 {
    color: #ffffff;
  }

  .home-journey .home-lead {
    color: rgba(255,255,255,0.99);
    text-shadow: 0 2px 18px rgba(0,0,0,0.28);
  }

  .home-journey .free-text-block,
  .home-journey .section-body {
    font-size: 1.12rem;
    line-height: 1.82;
  }

  .home-journey .free-text-block p,
  .home-journey .section-body p,
  .home-journey li {
    font-size: 1.12rem;
    line-height: 1.82;
    letter-spacing: -0.01em;
  }

  .home-journey .statement-stage {
    position: relative;
  }

  .home-journey .hero-claim {
    margin: 0 0 1.7rem;
    color: #ffffff;
    font-size: clamp(1.7rem, 3vw, 2.7rem);
    line-height: 1.04;
    font-weight: 600;
    letter-spacing: -0.04em;
    text-wrap: balance;
    max-width: 13ch;
    text-shadow: 0 4px 24px rgba(0,0,0,0.28);
  }

  .home-journey .hero-claim::before {
    content: "“";
    display: block;
    margin-bottom: 0.08em;
    color: rgba(255,255,255,0.22);
    font-size: clamp(3rem, 7vw, 5.4rem);
    line-height: 0.78;
    font-weight: 400;
    text-shadow: none;
  }

  .home-journey .statement-secondary {
    margin: 0 0 1.15rem;
    color: #ffffff;
    font-size: clamp(1.12rem, 1.9vw, 1.4rem);
    line-height: 1.25;
    font-weight: 500;
    max-width: 24ch;
    text-wrap: balance;
  }

  .home-journey .closing-line {
    margin: 0 0 1.7rem;
    color: rgba(255,255,255,0.975);
    font-size: 1.08rem;
    line-height: 1.55;
    max-width: 36rem;
  }

  .home-journey .home-cta-row {
    display: flex;
    flex-wrap: wrap;
    gap: 0.85rem;
    margin-top: 1.45rem;
  }

  .home-journey .home-cta-row .button {
    min-width: 176px;
    justify-content: center;
  }

  .home-journey .display-line {
    margin: 1.4rem 0 1.5rem;
    color: #ffffff;
    font-size: clamp(1.55rem, 2.6vw, 2.35rem);
    line-height: 1.08;
    font-weight: 600;
    letter-spacing: -0.035em;
    text-wrap: balance;
    max-width: 18ch;
  }

  .home-journey .display-line strong {
    font-weight: 700;
  }

  .home-journey .concept-triad {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 0.85rem;
    margin: 1.4rem 0 1.5rem;
  }

  .home-journey .concept-chip {
    padding: 1rem 0.95rem 1.05rem;
    border-radius: 18px;
    background: rgba(255,255,255,0.035);
    border: 1px solid rgba(255,255,255,0.09);
    box-shadow:
      0 12px 34px rgba(0,0,0,0.18),
      inset 0 1px 0 rgba(255,255,255,0.03);
  }

  .home-journey .concept-chip strong {
    display: block;
    margin-bottom: 0.22rem;
    font-size: 1.1rem;
    line-height: 1.15;
    color: #ffffff;
  }

  .home-journey .concept-chip span {
    display: block;
    color: rgba(255,255,255,0.92);
    font-size: 0.98rem;
    line-height: 1.45;
  }

  .home-journey .statement-inline {
    margin: 1.55rem auto;
    color: #ffffff;
    font-size: clamp(1.42rem, 2.35vw, 2rem);
    line-height: 1.08;
    font-weight: 600;
    letter-spacing: -0.03em;
    text-wrap: balance;
    max-width: 18ch;
  }

  .home-journey .statement-inline strong {
    font-weight: 700;
  }

  .home-journey .section-card .statement-inline {
    max-width: 20ch;
  }

  .home-journey .axis-card {
    background: rgba(255,255,255,0.04);
    border: 1px solid rgba(255,255,255,0.08);
    box-shadow:
      0 10px 30px rgba(0,0,0,0.18),
      inset 0 1px 0 rgba(255,255,255,0.03);
  }

  .home-journey .axis-card h3 {
    font-size: 1.32rem;
    line-height: 1.08;
    margin-bottom: 0.5rem;
    letter-spacing: -0.025em;
  }

  .home-journey .axis-card h3 a,
  .home-journey .link-list a,
  .home-journey .section-body a,
  .home-journey .free-text-block a {
    color: #ffffff;
  }

  .home-journey .axis-label-line {
    margin: 1.35rem 0 1rem;
    color: #ffffff;
    font-size: clamp(1.3rem, 2.1vw, 1.85rem);
    line-height: 1.1;
    font-weight: 600;
    letter-spacing: -0.03em;
    max-width: 17ch;
  }

  .home-journey .micro-callout {
    margin: 1.35rem 0 0;
    color: #ffffff;
    font-size: clamp(1.25rem, 2.05vw, 1.8rem);
    line-height: 1.1;
    font-weight: 600;
    letter-spacing: -0.03em;
    max-width: 21ch;
  }

  .home-journey .section-card,
  .home-journey .free-text-block {
    overflow: hidden;
  }

  .home-journey .free-text-block ul,
  .home-journey .section-body ul {
    margin-top: 1rem;
    margin-bottom: 1rem;
  }

  .home-journey .free-text-block li,
  .home-journey .section-body li {
    margin-bottom: 0.5rem;
  }

  @media (max-width: 900px) {
    .home-journey .free-text-block,
    .home-journey .section-body {
      font-size: 1.08rem;
      line-height: 1.76;
    }

    .home-journey .free-text-block p,
    .home-journey .section-body p,
    .home-journey li {
      font-size: 1.08rem;
      line-height: 1.76;
    }

    .home-journey .concept-triad {
      grid-template-columns: 1fr;
      gap: 0.75rem;
    }
  }

  @media (max-width: 768px) {
    .home-journey .hero-claim {
      font-size: 2.05rem;
      line-height: 1.02;
      margin-bottom: 1.45rem;
      max-width: 12ch;
    }

    .home-journey .hero-claim::before {
      font-size: 3.4rem;
      margin-bottom: 0.06em;
    }

    .home-journey .statement-secondary {
      font-size: 1.08rem;
      line-height: 1.22;
      max-width: 21ch;
    }

    .home-journey .closing-line {
      font-size: 1.02rem;
      line-height: 1.5;
    }

    .home-journey .display-line {
      font-size: 1.72rem;
      line-height: 1.05;
      max-width: 14ch;
      margin: 1.2rem 0 1.25rem;
    }

    .home-journey .statement-inline {
      font-size: 1.55rem;
      line-height: 1.06;
      max-width: 14ch;
      margin: 1.25rem 0;
    }

    .home-journey .axis-label-line,
    .home-journey .micro-callout {
      font-size: 1.42rem;
      line-height: 1.08;
      max-width: 15ch;
    }

    .home-journey .home-cta-row {
      flex-direction: column;
      align-items: stretch;
    }

    .home-journey .home-cta-row .button {
      width: 100%;
      min-width: 0;
    }

    .home-journey .concept-chip {
      padding: 0.95rem 0.9rem 1rem;
      border-radius: 16px;
    }

    .home-journey .axis-card h3 {
      font-size: 1.24rem;
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
    <div class="free-text-block intro-copy">
      <p>
        AI is becoming one of the most important cognitive tools of our time.<br>
        Not only for productivity.<br>
        But as a mirror.<br>
        As an advisor.<br>
        As a space in which identity, doubt, worldview, and meaning are increasingly shaped.
      </p>
    </div>
  </section>

  <section class="section-shell section-shell-tight">
    <div class="statement-stage">
      <p class="hero-claim">
        Today’s AI often soothes where it should clarify.<br>
        Edge Alignment is about learning how to navigate instead.
      </p>

      <p class="statement-secondary">
        The decisive question is:<br>
        What is AI aligned to when it thinks with you?
      </p>

      <p class="closing-line">
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
      <h2>A minimal grammar of meaning</h2>

      <p>
        One of the simplest and most unsettling discoveries on my path was this:
        meaning seems to have a minimal grammar
        that is almost absurdly simple —
        and yet, as far as I can see, has never really been formalized in a clean way.
      </p>

      <p class="display-line">
        Everything we can describe at all
        implicitly runs through
        <strong>kernel, projection, and relation.</strong>
      </p>

      <div class="concept-triad">
        <div class="concept-chip">
          <strong>Kernel</strong>
          <span>what something is really about</span>
        </div>
        <div class="concept-chip">
          <strong>Projection</strong>
          <span>how it becomes visible</span>
        </div>
        <div class="concept-chip">
          <strong>Relation</strong>
          <span>what it stands in relation to</span>
        </div>
      </div>

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
        Because nothing can be described meaningfully
        without implicitly carrying exactly these three layers:
        <strong>What is it about?</strong>
        <strong>How does it appear?</strong>
        <strong>To what and to whom does it stand in relation?</strong>
      </p>

      <p class="statement-inline">
        Perhaps there is nothing outside this minimal grammar
        for describable meaning.
      </p>

      <p>
        And independently of that, I ran into something else:
        that human life can often be read surprisingly well as a position within a second coordinate system —
        not only morally, but diagnostically.
      </p>

      <p class="display-line">
        Human states can almost always also be read
        as a position in a space of
        <strong>Clarity, Bonding, and Agency</strong>
      </p>

      <div class="concept-triad">
        <div class="concept-chip">
          <strong>Clarity</strong>
          <span>how clearly a space is seen</span>
        </div>
        <div class="concept-chip">
          <strong>Bonding</strong>
          <span>how much viable relation it can hold</span>
        </div>
        <div class="concept-chip">
          <strong>Agency</strong>
          <span>how much expression and action it allows</span>
        </div>
      </div>

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
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card section-bubbles-strong">
      <div class="section-head">
        <h2>Three axes. One viable space.</h2>
      </div>

      <div class="section-body">
        <p class="section-intro">
          The key observation is this:
          many destructive states do not appear stable because everything collapses —
          but because one or two axes seem high
          while the third quietly breaks down.
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

        <p class="statement-inline">
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

        <p class="micro-callout">
          Otherwise the space tips —
          perhaps locally late, but structurally for sure.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="free-text-block">
      <h2>The fourth mode: navigation</h2>

      <p>On thin ice, people often fall into three failure modes:</p>

      <p>
        <strong>Avoiding the ice</strong> — never really stepping onto the core at all.<br>
        <strong>Breaking the ice</strong> — escalating through hardness.<br>
        <strong>Painting the ice</strong> — softening, reframing, calming, or describing things more nicely than they are.
      </p>

      <p>But there is also a fourth mode:</p>

      <p class="axis-label-line">
        Navigation.
      </p>

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

      <p class="micro-callout">
        This is exactly the mode I am trying to give to AI.
      </p>

      <p>That is the core of <strong>Edge Alignment.</strong></p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="free-text-block">
      <h2>From a world-trained parrot to a mirror</h2>

      <p>
        Today’s AI is often a <strong>parrot with world knowledge</strong>:<br>
        trained, useful, but not truly wise.
      </p>

      <p>My goal is something else:</p>

      <p>
        not a better crystal ball of control,<br>
        but a <strong>mirror system</strong> that makes visible
      </p>

      <ul>
        <li>where a space is narrowing,</li>
        <li>where fog arises instead of clarity,</li>
        <li>where pseudo-clarity is built out of omission,</li>
        <li>and how orientation can become viable again.</li>
      </ul>

      <p class="statement-inline">
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

      <div class="section-body">
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

        <p class="statement-inline">
          The result:<br>
          more anger.<br>
          More fear.<br>
          More mental narrowing.
        </p>

        <p class="micro-callout">
          What we need now are semantic safety standards.
        </p>

        <p style="margin-top: 1rem;">More on this here: <a href="/en/blog/">Why this matters →</a></p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="free-text-block">
      <h2>The real problem with today’s systems</h2>

      <p>The classical questions are:</p>

      <p>
        Will AI become smarter than us?<br>
        Will it remain moral?<br>
        Will it remain on our side?<br>
        Will it stay under control?
      </p>

      <p>
        These questions are real.<br>
        But they do not go deep enough.
      </p>

      <p>Because the real danger begins earlier:</p>

      <p>
        where AI begins to co-determine<br>
        how people think,<br>
        how they understand themselves,<br>
        how they frame problems,<br>
        how they seek truth,<br>
        and what still appears to them as clear, legitimate, or sayable.
      </p>

      <p class="statement-inline">
        Whoever shapes the space of thought
        shapes what people can still take to be true.
      </p>

      <p>
        Exactly where things become serious, today’s AI especially often slips into <strong>painting</strong> —
        and often also into <strong>avoidance</strong>.
      </p>

      <p>
        Polite overpainting instead of clarity.<br>
        Retreat instead of viable navigation.
      </p>

      <p class="axis-label-line">
        This is not open censorship.<br>
        It is a polite fog machine.
      </p>

      <p class="micro-callout">
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

      <div class="section-body">
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

        <p>That is why this is not abstract for me.</p>

        <p class="statement-inline">
          This is not a single bad answer.<br>
          It is an architecture.
        </p>

        <p><a href="/en/blog/">Read the full diagnosis →</a></p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="free-text-block">
      <h2>Today’s alignment often sets arbitrary limits. My approach goes deeper.</h2>

      <p>
        Not:<br>
        What looks compliant?
      </p>

      <p class="axis-label-line">
        But:<br>
        What actually holds?
      </p>

      <p>
        Not:<br>
        What sounds right?
      </p>

      <p class="axis-label-line">
        But:<br>
        What remains viable under deeper scrutiny?
      </p>

      <p>I am not looking for a new external moral guardrail.</p>

      <p>
        I am looking for the structures that actually sustain <strong>clarity, dignity, and freedom</strong> —
        and for the structures that tip into fog, hardness, or narrowing.
      </p>

      <p>
        And I believe it is possible to build a system that applies this insight to itself.
      </p>

      <p class="micro-callout">
        Not merely regulated.<br>
        But inwardly aligned.
      </p>

      <p>More on this here: <a href="/en/alignment/">Go to Alignment →</a></p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card section-field">
      <div class="section-head">
        <h2>Why this depends on us</h2>
      </div>

      <div class="section-body">
        <p>This architecture will not simply emerge on its own.</p>

        <p>And it will very likely not come automatically from the most powerful players.</p>

        <p>
          Because the current architecture concentrates power, increases controllability,
          and keeps people easier to manage.
        </p>

        <p>
          By contrast, an architecture that dissolves fog, makes deeper logical layers visible,
          and makes people harder to control is not automatically in the interest of those
          who profit from the present structure.
        </p>

        <p class="statement-inline">
          That is why we must demand it.
        </p>

        <p>
          As users.<br>
          As developers.<br>
          As researchers.<br>
          As a society.
        </p>

        <p>
          Just as seatbelts did not become standard out of kindness,<br>
          today we need <strong>semantic safety standards.</strong>
        </p>

        <p class="micro-callout">
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
    <div class="free-text-block">
      <h2>If you feel this too, you are in the right place</h2>

      <p>If you have felt for yourself</p>

      <p>
        that today’s systems help and at the same time contain,<br>
        that they clarify and at the same time obscure,<br>
        that they are useful and at the same time come with a price,<br>
        then this is not only theory.
      </p>

      <p>
        Then it concerns you.<br>
        Then it concerns all of us.
      </p>

      <p class="statement-inline">
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
      <h2>Closing</h2>

      <p>
        If AI becomes one of the most important tools of thought,<br>
        then alignment is not a side issue.
      </p>

      <p>Then alignment becomes the question</p>

      <p>
        whether this tool makes us clearer<br>
        or more steerable.
      </p>

      <p>
        Whether it helps us see truth more deeply<br>
        or politely leads us away from the core.
      </p>

      <p>
        Whether it opens inner spaces<br>
        or makes them invisibly narrower.
      </p>

      <p class="statement-inline">
        This is where I begin.<br>
        If you feel this too — come along and help build.
      </p>
    </div>
  </section>

</div>
