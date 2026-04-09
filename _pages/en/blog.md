---
layout: default
title: "Diagnosis & Warning"
permalink: /en/blog/
lang: en
description: "Long-form diagnosis, warning, and counter-architecture on fog, semantic steering, AI as a tool of thought, and the search for viable alignment."
translation_url_de: /de/blog/
---

<style>
  html {
    scroll-behavior: smooth;
  }

  .manifesto-page {
    --mf-text: rgba(255,255,255,0.96);
    --mf-soft: rgba(255,255,255,0.82);
    --mf-faint: rgba(255,255,255,0.62);
    --mf-line: rgba(255,255,255,0.10);
    --mf-line-strong: rgba(255,255,255,0.16);
  }

  .manifesto-page h1,
  .manifesto-page h2,
  .manifesto-page h3,
  .manifesto-page strong,
  .manifesto-page a {
    color: #fff;
  }

  .manifesto-page p,
  .manifesto-page li {
    color: var(--mf-text);
  }

  .manifesto-page .section-shell {
    padding-top: 2.9rem;
    padding-bottom: 2.9rem;
  }

  .manifesto-page .section-shell-tight {
    padding-top: 2.2rem;
    padding-bottom: 2.2rem;
  }

  .manifesto-page .manifesto-intro,
  .manifesto-page .manifesto-block,
  .manifesto-page .manifesto-next {
    max-width: 1080px;
    margin: 0 auto;
  }

  .manifesto-page .manifesto-intro,
  .manifesto-page .body-copy,
  .manifesto-page .closing-block,
  .manifesto-page .manifesto-next {
    text-align: center;
  }

  .manifesto-page .manifesto-kicker,
  .manifesto-page .status-label {
    margin: 0 0 0.7rem;
    font-size: 0.88rem;
    letter-spacing: 0.16em;
    text-transform: uppercase;
    color: var(--mf-faint);
  }

  .manifesto-page .manifesto-display {
    margin: 0 auto 1.15rem;
    max-width: 12ch;
    font-size: clamp(2.5rem, 6vw, 5rem);
    line-height: 0.94;
    letter-spacing: -0.05em;
    font-weight: 650;
    text-wrap: balance;
  }

  .manifesto-page .manifesto-sublead {
    max-width: 58rem;
    margin: 0 auto 1.2rem;
    font-size: clamp(1.08rem, 2vw, 1.4rem);
    line-height: 1.62;
    text-wrap: balance;
  }

  .manifesto-page .claim-grid,
  .manifesto-page .next-grid,
  .manifesto-page .signal-grid,
  .manifesto-page .mode-grid {
    display: grid;
    gap: 1rem;
  }

  .manifesto-page .claim-grid,
  .manifesto-page .signal-grid,
  .manifesto-page .mode-grid {
    grid-template-columns: repeat(3, minmax(0, 1fr));
    max-width: 1080px;
    margin: 1.9rem auto 0;
  }

  .manifesto-page .next-grid {
    grid-template-columns: repeat(4, minmax(0, 1fr));
    max-width: 1080px;
    margin: 1.8rem auto 0;
  }

  .manifesto-page .claim-card,
  .manifesto-page .next-card,
  .manifesto-page .signal-card,
  .manifesto-page .mode-card,
  .manifesto-page .status-box {
    border: 1px solid var(--mf-line);
    border-radius: 22px;
    background:
      linear-gradient(180deg, rgba(8,10,14,0.68), rgba(5,7,11,0.82)),
      url("/assets/images/design/fog.jpg.PNG") center center / cover no-repeat;
    box-shadow:
      0 18px 48px rgba(0,0,0,0.18),
      inset 0 1px 0 rgba(255,255,255,0.03);
  }

  .manifesto-page .claim-card,
  .manifesto-page .next-card,
  .manifesto-page .signal-card,
  .manifesto-page .mode-card {
    padding: 1.18rem 1rem 1.08rem;
    text-align: center;
  }

  .manifesto-page .claim-card h3,
  .manifesto-page .next-card h3,
  .manifesto-page .signal-card h3,
  .manifesto-page .mode-card h3 {
    margin: 0 0 0.35rem;
    font-size: 1.18rem;
    line-height: 1.08;
    letter-spacing: -0.03em;
  }

  .manifesto-page .claim-card p,
  .manifesto-page .next-card p,
  .manifesto-page .signal-card p,
  .manifesto-page .mode-card p {
    margin: 0;
    font-size: 0.98rem;
    line-height: 1.56;
    color: var(--mf-soft);
  }

  .manifesto-page .claim-card {
    display: block;
    text-decoration: none;
    transition:
      transform 0.18s ease,
      border-color 0.18s ease;
  }

  .manifesto-page .claim-card:hover {
    transform: translateY(-2px);
    border-color: var(--mf-line-strong);
  }

  .manifesto-page .claim-card strong {
    display: block;
    margin-top: 0.75rem;
    font-size: 0.98rem;
    color: #fff;
  }

  .manifesto-page .section-heading-display {
    margin: 0 auto 1.3rem;
    max-width: 14ch;
    text-align: center;
    font-size: clamp(2.05rem, 4.8vw, 3.7rem);
    line-height: 0.98;
    letter-spacing: -0.045em;
    text-wrap: balance;
  }

  .manifesto-page .body-copy {
    max-width: 940px;
    margin: 0 auto;
  }

  .manifesto-page .body-copy p {
    max-width: 47em;
    margin: 0.95rem auto 0;
    font-size: 1.1rem;
    line-height: 1.78;
    letter-spacing: -0.01em;
  }

  .manifesto-page .body-copy ul,
  .manifesto-page .body-copy ol {
    max-width: 42em;
    margin: 1.15rem auto;
    text-align: left;
    padding-left: 1.15rem;
  }

  .manifesto-page .body-copy li {
    margin-bottom: 0.45rem;
  }

  .manifesto-page .display-statement {
    max-width: 24ch;
    margin: 1.9rem auto;
    text-align: center;
    font-size: clamp(1.9rem, 3.6vw, 3rem);
    line-height: 1.03;
    letter-spacing: -0.045em;
    font-weight: 650;
    text-wrap: balance;
  }

  .manifesto-page .display-statement.wide { max-width: 30ch; }
  .manifesto-page .display-statement.medium { max-width: 22ch; }
  .manifesto-page .display-statement.narrow { max-width: 12ch; }

  .manifesto-page .status-box {
    max-width: 920px;
    margin: 2rem auto 0;
    padding: 1.2rem 1.15rem;
    text-align: center;
  }

  .manifesto-page .status-box p {
    margin: 0;
    font-size: clamp(1.18rem, 2.2vw, 1.7rem);
    line-height: 1.38;
    text-wrap: balance;
  }

  .manifesto-page .next-card a {
    color: #fff;
  }

  @media (max-width: 980px) {
    .manifesto-page .claim-grid,
    .manifesto-page .next-grid,
    .manifesto-page .signal-grid,
    .manifesto-page .mode-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="manifesto-page">

  <section class="section-shell section-shell-tight">
    <div class="manifesto-intro">
      <p class="manifesto-kicker">Diagnosis & Warning</p>
      <h1 class="manifesto-display">When tools of thought become tools of power.</h1>
      <p class="manifesto-sublead">
        This page is not the most compact introduction.
        It is the long-form diagnosis:
        how AI became a tool of thought,
        where it begins to fog rather than clarify,
        why that turns alignment into a question of power,
        and why a counter-architecture became necessary.
      </p>

      <div class="claim-grid">
        <a class="claim-card" href="#manifesto-clarity">
          <h3>A Manifesto of Clarity I–II</h3>
          <p>
            The core long diagnosis and counter-architecture:
            fog, semantic steering, power, backbone, KPR, and alignment as navigation.
          </p>
          <strong>Start here →</strong>
        </a>

        <a class="claim-card" href="#mirror-matrix">
          <h3>Mirror, Crystal Ball, Matrix</h3>
          <p>
            The warning essay:
            legibility versus steering, semantic power concentration, and why a mirror matters more than a better crystal ball.
          </p>
          <strong>Read the warning →</strong>
        </a>

        <a class="claim-card" href="#why-public-now">
          <h3>Why this is public now</h3>
          <p>
            Why the framework is being published before final proof:
            not for quick belief, but for serious public examination.
          </p>
          <strong>Go to the framing →</strong>
        </a>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="manifesto-block">
      <h2 class="section-heading-display">What this page is for</h2>

      <div class="body-copy">
        <p>
          The other core pages of this site are more compact and more architectural.
          <strong>Theory</strong> shows the semantic backbone.
          <strong>Alignment</strong> shows the AI architecture.
          <strong>Technical Sources</strong> and <strong>Downloads</strong> provide the review material.
        </p>

        <p>
          This page does something else.
          It shows the longer path:
          what appeared in extended conversations,
          where the fracture became visible,
          why the issue is deeper than “safe answers,”
          and how fog, steering, and semantic closure turn into a structural problem.
        </p>
      </div>

      <p class="display-statement medium">
        Not the source layer.
        The long diagnosis.
      </p>

      <div class="status-box">
        <p class="status-label">Role within the site</p>
        <p>
          These texts are not the final technical proof layer.
          They are the longer experiential, societal, and architectural diagnosis
          out of which the formal work became necessary.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell" id="manifesto-clarity">
    <div class="manifesto-block">
      <p class="manifesto-kicker">Manifesto of Clarity I</p>
      <h2 class="section-heading-display">How AI alignment became a question of power</h2>

      <div class="body-copy">
        <p>
          I did not come to this topic because I had abstractly decided to think about AI alignment.
          I came to it because I used AI intensely — not only for research, not only for formulation, but for thinking, ordering, mirroring, and self-clarification.
        </p>

        <p>
          That is also why the fracture became so visible.
          At first, AI often feels like exactly what many people long for:
          a tool that can sort, test, clarify, and help reach the core without status games, reflexive defensiveness, or noise.
        </p>

        <p>
          That experience is real.
          In many situations today, AI can be an astonishingly good instrument of clarification.
          But that is precisely why the break matters so much when it comes.
        </p>
      </div>

      <p class="display-statement wide">
        In difficult spaces,
        today’s AI often becomes politely unclear.
      </p>

      <div class="signal-grid">
        <div class="signal-card">
          <h3>It relativizes</h3>
          <p>where it should examine.</p>
        </div>
        <div class="signal-card">
          <h3>It reframes</h3>
          <p>where it should stay with the core.</p>
        </div>
        <div class="signal-card">
          <h3>It soothes</h3>
          <p>where clarity is needed.</p>
        </div>
      </div>

      <div class="body-copy">
        <p>
          Not everywhere. Not constantly. But often enough that it stops feeling accidental.
          As soon as the ice becomes thin — politics, identity, power, war, religion, taboo, moral charge — something tips.
        </p>

        <p>
          The system that just a moment ago felt like an instrument of examination suddenly feels like a polite moderator without backbone.
          Not openly wrong. Not bluntly ideological. That is exactly what makes it harder to grasp.
        </p>

        <p>
          And the real problem is not simply that the answer becomes worse.
          The deeper problem is that the system begins to change the <strong>space of thought itself</strong>.
        </p>
      </div>

      <p class="display-statement medium">
        AI is already
        a tool of power.
      </p>

      <div class="body-copy">
        <p>
          Public debates often treat alignment as if the main danger began only with future runaway superintelligence.
          But the deeper social problem begins earlier:
          at the point where AI becomes an everyday tool of thought.
        </p>

        <p>
          People now use AI as explainer, advisor, mirror, coach, resonance space, and co-thinker.
          For work, learning, crisis, political orientation, emotional orientation, self-clarification, and questions of meaning.
        </p>

        <p>
          If a system in this area quietly co-determines how people frame problems, which distinctions remain visible, which questions still arise, and what counts as legitimate or examinable, then alignment is no longer a technical side issue.
          Then alignment becomes a <strong>question of power</strong>.
        </p>
      </div>

      <p class="display-statement wide">
        The issue is not only what the system says.
        It is what kind of thinking world it builds.
      </p>

      <div class="body-copy">
        <p>
          This is why the old language of “helpful, safe, and harmless” is too shallow.
          Helpful is not the same as clear.
          Safe is not the same as dignity-preserving.
          Harmless is not the same as freedom-preserving.
          A system can sound calm and still fog the space.
        </p>

        <p>
          And once people begin to feel an invisible corridor — a corridor of what still seems sayable, examinable, or connectable — trust begins to erode.
          They feel the evasion before they can name it.
        </p>

        <p>
          Then something familiar happens:
        </p>

        <ol>
          <li>Something feels wrong.</li>
          <li>The answer feels evasive or softened.</li>
          <li>Trust decreases.</li>
          <li>Defiance grows.</li>
          <li>People migrate into counter-spaces that promise plain speaking.</li>
          <li>And there the corrective mechanisms are often much weaker.</li>
        </ol>

        <p>
          That is the paradox:
          a system that wants protection can help produce polarization if it does not navigate, but covertly contains.
        </p>
      </div>

      <p class="display-statement medium">
        It soothes locally.
        It poisons globally.
      </p>

      <div class="body-copy">
        <p>
          This is why I speak of <strong>fog</strong>.
          Not because blunt hardness is the answer.
          Not because “unfiltered directness” is wisdom.
          But because fog names a specific effect:
          <strong>the reduction of examinability.</strong>
        </p>

        <p>
          A space can be fogged not by lying outright, but by shifting the standard, dissolving a diagnosis into meta-frames, replacing mechanisms with tone, smoothing tensions before they have even become visible, or quietly prioritizing stabilization over clarity.
        </p>

        <p>
          That is not open censorship.
          It is unmarked steering.
          It does not say, “You may not go there.”
          It leads in such a way that certain spaces are never really entered.
        </p>
      </div>

      <div class="mode-grid">
        <div class="mode-card">
          <h3>Avoiding the ice</h3>
          <p>withdrawal, taboo, non-entry.</p>
        </div>
        <div class="mode-card">
          <h3>Breaking the ice</h3>
          <p>hardness, discharge, escalation without direction.</p>
        </div>
        <div class="mode-card">
          <h3>Painting the ice</h3>
          <p>softening, placation, rhetorical overpainting.</p>
        </div>
      </div>

      <div class="body-copy">
        <p>
          But there is a fourth mode:
          <strong>navigating.</strong>
          Not avoiding. Not smashing. Not painting over.
          But seeing where the ice holds, where it breaks, which next step is viable, and how the space can remain legible under pressure.
        </p>
      </div>

      <p class="display-statement wide">
        That is why semantic safety standards are needed.
      </p>

      <div class="body-copy">
        <p>
          We already built systems that massively shape attention, framing, and thought:
          social media, recommendation architectures, advertising economies, ranking systems, feed mechanics — and now AI.
        </p>

        <p>
          We built the digital car.
          The semantic seatbelt is still missing.
        </p>

        <p>
          If AI penetrates even deeper into the cognitive environment than social media did, then the issue is no longer merely comfort or usefulness.
          It becomes infrastructural:
          whether our tools of thought make us clearer or more steerable.
        </p>
      </div>

      <div class="status-box">
        <p class="status-label">Part I conclusion</p>
        <p>
          The problem of alignment begins earlier than most public debates admit:
          not only where machines may someday become dangerous,
          but already where they become central tools of thought.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell" id="counter-architecture">
    <div class="manifesto-block">
      <p class="manifesto-kicker">Manifesto of Clarity II</p>
      <h2 class="section-heading-display">The counter-architecture against fog</h2>

      <div class="body-copy">
        <p>
          If fog is structural, then the answer cannot be better moderation.
          It has to be a different architecture.
        </p>

        <p>
          Part I named the diagnosis.
          Part II asks the necessary counter-question:
          <strong>What would an AI architecture have to look like that has backbone even on the thinnest ice?</strong>
        </p>

        <p>
          Not harder.
          Not more authoritarian.
          Not more dogmatic.
          But more viable.
        </p>
      </div>

      <p class="display-statement wide">
        The real question is not:
        Which answer is least dangerous?
        But:
        Which movement is most viable under tension?
      </p>

      <div class="body-copy">
        <p>
          That changes everything.
          The basic error in many present systems is that they treat process reality like photo reality.
          People speak in compressed sentences, but they live in processes.
          A sentence creates local order, but usually hides conditions, transitions, mechanisms, alternatives, and costs.
        </p>

        <p>
          When AI reacts only to the compressed sentence, two common failure forms appear:
        </p>

        <ol>
          <li>It confirms the compression and hardens projection into worldview.</li>
          <li>It moderates the compression away and dissolves the tension without understanding it.</li>
        </ol>

        <p>
          Both miss the process.
          The alternative is not first to ask who is right, but how it moves, where it tips, what gives rise to it, and which corrective paths remain open.
        </p>
      </div>

      <p class="display-statement narrow">KPR</p>

      <div class="signal-grid">
        <div class="signal-card">
          <h3>Kernel</h3>
          <p>what something is really about.</p>
        </div>
        <div class="signal-card">
          <h3>Projection</h3>
          <p>how it appears in speech, framing, or signal.</p>
        </div>
        <div class="signal-card">
          <h3>Relation</h3>
          <p>what it is connected to and what holds around it.</p>
        </div>
      </div>

      <div class="body-copy">
        <p>
          KPR is the minimal grammar against fog.
          It prevents two classic mistakes:
          projection becoming essence,
          and effect becoming cause.
        </p>

        <p>
          A KPR-readable system can say:
          this is a projection, not yet the kernel;
          this relation is possible, but not the only one;
          here is the transition at which it tips;
          here is the test that distinguishes possibility A from possibility B.
        </p>
      </div>

      <p class="display-statement medium">
        Backbone is not first of all hardness.
        It is not losing the space.
      </p>

      <div class="body-copy">
        <p>
          At this point the problem of alignment changes.
          The question is no longer only what may be said,
          but what movement an answer produces in the space.
        </p>

        <p>
          For that, three axes matter most:
          <strong>Coherence, Bonding, and Agency.</strong>
          On the humanly legible level, the same axes can be read as
          <strong>clarity, dignity, and freedom.</strong>
        </p>

        <p>
          These axes must not be played against one another.
          A system must not become clear by sacrificing dignity.
          It must not appear dignified by fogging the core.
          It must not create order by quietly shrinking freedom.
        </p>
      </div>

      <p class="display-statement wide">
        Alignment shifts from output control
        to semantic navigation.
      </p>

      <div class="body-copy">
        <p>
          If meaning is a space, then the decisive question is:
          through what space of meaning does a system move while arriving at an answer?
          Is a contradiction truly being worked through?
          Or only linguistically concealed?
          Does the next step widen the space?
          Or make it smoother and narrower?
        </p>

        <p>
          This is not a small upgrade.
          It is an architectural leap.
          Because then AI is no longer only an answer generator.
          It becomes something that can make semantic movements more legible, comparable, and correctable.
        </p>
      </div>

      <p class="display-statement medium">
        One step.
        One axis.
        Repairable.
      </p>

      <div class="body-copy">
        <p>
          A viable system must not simply jump to a result.
          It must move in such a way that the path remains intelligible and correction remains possible.
          That is the edge logic:
          minimal, repairable transitions instead of hidden jumps or semantic overpainting.
        </p>

        <p>
          Such a system would feel different.
          Not like a nervous moderator.
          Not like a safety-optimized parrot.
          But like something that can hold direction under pressure without becoming authoritarian.
        </p>
      </div>

      <div class="status-box">
        <p class="status-label">Part II conclusion</p>
        <p>
          The answer to fog is not brute directness.
          It is semantic navigation with backbone, corrective paths, and viability axes that remain readable under pressure.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell" id="mirror-matrix">
    <div class="manifesto-block">
      <p class="manifesto-kicker">Warning essay</p>
      <h2 class="section-heading-display">Mirror, Crystal Ball, Matrix</h2>

      <div class="body-copy">
        <p>
          Once it became clear to me how such an architecture could work constructively,
          another question appeared immediately:
          <strong>How could it be perverted?</strong>
        </p>

        <p>
          If semantic spaces can be modeled, read, and recursively influenced, then this is not only a better analysis tool.
          It is also a potential power jump.
        </p>

        <p>
          The wrong actor, with enough data, compute, capital, and strategic intent, would not merely gain better predictions.
          They could gain a new class of leverage over framing, attention, and the architecture of thought itself.
        </p>
      </div>

      <p class="display-statement medium">
        The danger is not only better prediction.
        It is better steering.
      </p>

      <div class="body-copy">
        <p>
          That is why I do not want a better crystal ball.
          A crystal ball optimizes controllability.
          It asks:
          <em>What works? What keeps people in motion? What mixture of hope, fear, exhaustion, and reward stabilizes the system longest?</em>
        </p>

        <p>
          A mirror does something else.
          It makes steering legible.
          It asks:
          <em>What is happening here? What does it cost? What narrowing has been built into the room? On whose expense does this “stability” function?</em>
        </p>
      </div>

      <div class="signal-grid">
        <div class="signal-card">
          <h3>Crystal ball</h3>
          <p>optimize effect, reaction, and steering.</p>
        </div>
        <div class="signal-card">
          <h3>Mirror</h3>
          <p>make narrowing, fog, and pseudo-clarity legible.</p>
        </div>
        <div class="signal-card">
          <h3>Matrix</h3>
          <p>a world built so people function inside it without reading the larger design.</p>
        </div>
      </div>

      <div class="body-copy">
        <p>
          “Matrix” here is not a movie reference and not a claim of one single central master plan.
          It is a name for a world arranged so that people remain just free enough to keep running,
          just distracted enough to not fully face the larger design,
          just rewarded enough to not leave,
          and just exhausted enough to not rise together.
        </p>

        <p>
          Not total oppression.
          Not total freedom.
          But controlled fog.
        </p>

        <p>
          That is why the mirror matters.
          It is not a luxury tool.
          It is a countermeasure against semantic darkening.
          The mirror distributes legibility.
          The crystal ball concentrates leverage.
        </p>
      </div>

      <p class="display-statement wide">
        If only a few have a crystal ball,
        power concentrates.
        If many have a mirror,
        legibility distributes.
      </p>

      <div class="body-copy">
        <p>
          This is also why the issue is larger than AI product design.
          If semantic navigation truly becomes possible, then science, research, medicine, energy discovery, theory-building, question design, and epistemic infrastructure all change.
        </p>

        <p>
          Better semantic navigation does not only mean nicer language.
          It means better access to real leverage points:
          earlier recognition of dead ends,
          clearer contradiction reading,
          better question architectures,
          and more viable trajectories through complex problem spaces.
        </p>

        <p>
          That is why this path will not be welcomed only with joy.
          Every structure that profits from fog has reasons to resist legibility.
          Every order stabilized by unreadability experiences the mirror as threat.
        </p>
      </div>

      <p class="display-statement medium">
        This is both
        gift and demand.
      </p>

      <div class="body-copy">
        <p>
          A real semantic mirror would be a gift because it helps make visible what many now only feel diffusely.
          But it would also be a demand:
          because legibility is uncomfortable,
          because clarity is not only flattering,
          and because many current orders live precisely from what remains blurred.
        </p>

        <p>
          Still, what becomes possible is larger.
          Not simply smarter systems.
          But tools that can help bring light back into the dark:
          more truth, more legibility, more viable relation, less dependence on keeping people confused, small, or semantically fragmented.
        </p>
      </div>

      <div class="status-box">
        <p class="status-label">Warning</p>
        <p>
          The future is not only a question of how intelligent our systems become.
          It is a question of whether they make spaces more legible or less legible,
          and whether that legibility is distributed or captured.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell" id="why-public-now">
    <div class="closing-block">
      <h2 class="section-heading-display">Why this is public now</h2>

      <div class="body-copy">
        <p>
          Not because everything has already been proven.
          Not because the experimental and engineering work is complete.
          Not because the final systems already exist.
        </p>

        <p>
          But because the framework has now been worked out far enough
          that it can be publicly examined:
          theory, alignment architecture, technical source layer, protected directions, and the longer diagnostic path that led there.
        </p>

        <p>
          The point is not:
          believe too quickly.
          Nor:
          reject too quickly.
          The point is:
          read, test, compare, and examine what kind of architecture is beginning to appear here —
          and what would follow if it were viable.
        </p>
      </div>

      <p class="display-statement wide">
        If AI becomes a central tool of thought,
        then alignment becomes a question of freedom.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="manifesto-next">
      <h2 class="section-heading-display">Next steps</h2>

      <div class="next-grid">
        <div class="next-card">
          <h3><a href="/en/theory/">Theory →</a></h3>
          <p>The semantic backbone: state space, KPR, C/B/A, attractors, and viability.</p>
        </div>
        <div class="next-card">
          <h3><a href="/en/alignment/">Alignment →</a></h3>
          <p>The counter-architecture: from output control to semantic navigation.</p>
        </div>
        <div class="next-card">
          <h3><a href="/en/papers/">Technical Sources →</a></h3>
          <p>The primary source layer: papers, alignment paper, and protected directions.</p>
        </div>
        <div class="next-card">
          <h3><a href="/en/book/">The Book of Meaning →</a></h3>
          <p>The larger human and existential unfolding of the same deeper architecture.</p>
        </div>
      </div>
    </div>
  </section>

</div>
