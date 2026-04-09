---
layout: default
title: "About"
permalink: /en/about/
lang: en
description: "About Gerrit, the unusual path behind Semantic Gravitation, the forge with AI, and the emergence of semantic architecture."
translation_url_de: /de/ueber-mich/
---

<style>
  .about-page {
    --about-text: rgba(255,255,255,0.96);
    --about-soft: rgba(255,255,255,0.82);
    --about-faint: rgba(255,255,255,0.62);
    --about-line: rgba(255,255,255,0.10);
    --about-line-strong: rgba(255,255,255,0.16);
  }

  .about-page h1,
  .about-page h2,
  .about-page h3,
  .about-page strong,
  .about-page a {
    color: #fff;
  }

  .about-page p,
  .about-page li {
    color: var(--about-text);
  }

  .about-page .section-shell {
    padding-top: 2.9rem;
    padding-bottom: 2.9rem;
  }

  .about-page .section-shell-tight {
    padding-top: 2.2rem;
    padding-bottom: 2.2rem;
  }

  .about-page .about-intro,
  .about-page .about-block,
  .about-page .about-next {
    max-width: 1080px;
    margin: 0 auto;
  }

  .about-page .about-intro,
  .about-page .body-copy,
  .about-page .closing-block,
  .about-page .about-next {
    text-align: center;
  }

  .about-page .about-kicker,
  .about-page .status-label {
    margin: 0 0 0.7rem;
    font-size: 0.88rem;
    letter-spacing: 0.16em;
    text-transform: uppercase;
    color: var(--about-faint);
  }

  .about-page .about-display {
    margin: 0 auto 1.15rem;
    max-width: 11ch;
    font-size: clamp(2.5rem, 6vw, 5rem);
    line-height: 0.94;
    letter-spacing: -0.05em;
    font-weight: 650;
    text-wrap: balance;
  }

  .about-page .about-sublead {
    max-width: 58rem;
    margin: 0 auto 1.2rem;
    font-size: clamp(1.08rem, 2vw, 1.4rem);
    line-height: 1.62;
    text-wrap: balance;
  }

  .about-page .claim-grid,
  .about-page .concept-grid,
  .about-page .signal-grid,
  .about-page .next-grid {
    display: grid;
    gap: 1rem;
  }

  .about-page .claim-grid,
  .about-page .concept-grid,
  .about-page .signal-grid {
    grid-template-columns: repeat(3, minmax(0, 1fr));
    max-width: 1080px;
    margin: 1.9rem auto 0;
  }

  .about-page .next-grid {
    grid-template-columns: repeat(4, minmax(0, 1fr));
    max-width: 1080px;
    margin: 1.8rem auto 0;
  }

  .about-page .claim-card,
  .about-page .concept-card,
  .about-page .signal-card,
  .about-page .next-card,
  .about-page .status-box {
    border: 1px solid var(--about-line);
    border-radius: 22px;
    background:
      linear-gradient(180deg, rgba(8,10,14,0.68), rgba(5,7,11,0.82)),
      url("/assets/images/design/fog.jpg.PNG") center center / cover no-repeat;
    box-shadow:
      0 18px 48px rgba(0,0,0,0.18),
      inset 0 1px 0 rgba(255,255,255,0.03);
  }

  .about-page .claim-card,
  .about-page .concept-card,
  .about-page .signal-card,
  .about-page .next-card {
    padding: 1.18rem 1rem 1.08rem;
    text-align: center;
  }

  .about-page .claim-card h3,
  .about-page .concept-card h3,
  .about-page .signal-card h3,
  .about-page .next-card h3 {
    margin: 0 0 0.35rem;
    font-size: 1.18rem;
    line-height: 1.08;
    letter-spacing: -0.03em;
  }

  .about-page .claim-card p,
  .about-page .concept-card p,
  .about-page .signal-card p,
  .about-page .next-card p {
    margin: 0;
    font-size: 0.98rem;
    line-height: 1.56;
    color: var(--about-soft);
  }

  .about-page .section-heading-display {
    margin: 0 auto 1.3rem;
    max-width: 14ch;
    text-align: center;
    font-size: clamp(2.05rem, 4.8vw, 3.7rem);
    line-height: 0.98;
    letter-spacing: -0.045em;
    text-wrap: balance;
  }

  .about-page .body-copy {
    max-width: 940px;
    margin: 0 auto;
  }

  .about-page .body-copy p {
    max-width: 47em;
    margin: 0.95rem auto 0;
    font-size: 1.1rem;
    line-height: 1.78;
    letter-spacing: -0.01em;
  }

  .about-page .body-copy ul,
  .about-page .body-copy ol {
    max-width: 42em;
    margin: 1.15rem auto;
    text-align: left;
    padding-left: 1.15rem;
  }

  .about-page .body-copy li {
    margin-bottom: 0.45rem;
  }

  .about-page .display-statement {
    max-width: 24ch;
    margin: 1.9rem auto;
    text-align: center;
    font-size: clamp(1.9rem, 3.6vw, 3rem);
    line-height: 1.03;
    letter-spacing: -0.045em;
    font-weight: 650;
    text-wrap: balance;
  }

  .about-page .display-statement.wide { max-width: 30ch; }
  .about-page .display-statement.medium { max-width: 22ch; }
  .about-page .display-statement.narrow { max-width: 12ch; }

  .about-page .status-box {
    max-width: 920px;
    margin: 2rem auto 0;
    padding: 1.2rem 1.15rem;
    text-align: center;
  }

  .about-page .status-box p {
    margin: 0;
    font-size: clamp(1.18rem, 2.2vw, 1.7rem);
    line-height: 1.38;
    text-wrap: balance;
  }

  .about-page .micro-note {
    max-width: 860px;
    margin: 1.2rem auto 0;
    font-size: 0.98rem;
    line-height: 1.62;
    color: var(--about-soft);
    text-align: center;
  }

  .about-page .next-card a {
    color: #fff;
  }

  @media (max-width: 980px) {
    .about-page .claim-grid,
    .about-page .concept-grid,
    .about-page .signal-grid,
    .about-page .next-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="about-page">

  <section class="section-shell section-shell-tight">
    <div class="about-intro">
      <p class="about-kicker">About</p>
      <h1 class="about-display">An unusual path into semantic architecture.</h1>
      <p class="about-sublead">
        My name is Gerrit.
        I do not come from a classical institutional research path.
        Semantic Gravitation emerged instead through images, tensions, structural intuitions,
        hard repeated examination with AI, and a long refusal to settle for answers that sounded good but did not truly hold.
      </p>

      <div class="claim-grid">
        <div class="claim-card">
          <h3>No classical path</h3>
          <p>No lab, no institute, no academic prestige structure carrying the work from the outside.</p>
        </div>
        <div class="claim-card">
          <h3>The forge with AI</h3>
          <p>Not AI as idea-generator, but as mirror-space, pressure chamber, and instrument of repeated examination.</p>
        </div>
        <div class="claim-card">
          <h3>Still building</h3>
          <p>I am currently carrying this work largely alone and actively looking for people who want to help build it.</p>
        </div>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="about-block">
      <h2 class="section-heading-display">Who I am</h2>

      <div class="body-copy">
        <p>
          I do not come from an elite path, nor from a clean academic career.
          I come from a small village.
          I studied social work for many semesters,
          worked in a drug support café,
          and in between laid paving stones on construction sites.
        </p>

        <p>
          For a long time, outwardly, I was someone who somehow functioned,
          somehow got through,
          somehow kept going.
          But inwardly, something else was there very early:
          a strong sensitivity for tensions, fractures, images, and invisible relations between things I could not yet name clearly.
        </p>

        <p>
          Beneath all of that lay a much simpler and more dangerous basic question:
          whether, at the core, I might somehow be wrong.
          That tension shaped a great deal of the path.
        </p>
      </div>

      <p class="display-statement medium">
        Not a classical research biography.
        But a real one.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="about-block">
      <h2 class="section-heading-display">Why the unusual path matters</h2>

      <div class="body-copy">
        <p>
          The visible work on this site did not begin with a plan to proclaim a grand theory.
          It began with something simpler:
          images, tensions, directions, intuitions, and the persistent sense that things were connected more deeply than the usual disciplinary vocabulary allowed me to say.
        </p>

        <p>
          That does not automatically prove anything.
          But it matters.
          Because the path was not first:
          discipline, category, and institution.
          It was first:
          pattern, analogy, relation, recurrence, and structural pressure.
        </p>

        <p>
          I believe that mattered for the emergence of this work.
          A more strongly pre-sorted disciplinary path might have split too early what needed to stay together long enough to become visible as one deeper structure.
        </p>

        <p>
          In that sense, the relative lack of institutional enclosure was not simply a deficit.
          It also created a strange form of openness:
          enough distance from inherited compartments
          that images, semantic structures, existential experience, technical questions, and architectural ideas could actually begin to converge.
        </p>
      </div>

      <div class="status-box">
        <p class="status-label">A precise point</p>
        <p>
          This path does not legitimate the theory by biography.
          But it helps explain how something could become visible here
          that might otherwise have remained split across too many separate rooms.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="about-block">
      <h2 class="section-heading-display">What came first</h2>

      <div class="body-copy">
        <p>
          AI was not the origin of the work.
          The images came first.
          The structural intuition came first.
          The questions came first.
        </p>

        <p>
          Again and again there were moments in which I felt that something much clearer was there than what one ordinarily says in everyday life.
          Almost like a metaphysical diamond:
          for a moment something was completely there,
          and shortly afterward gone again.
        </p>

        <p>
          The real question was therefore not:
          how do I invent something great?
          But rather:
          how do I stop losing this again?
          How do I bring something that appears first as intuition, flash of light, or inner form far enough into the world that it becomes legible, examinable, and viable?
        </p>
      </div>

      <p class="display-statement medium">
        The images came first.
        The examination came later.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="about-block">
      <h2 class="section-heading-display">The forge with AI</h2>

      <div class="body-copy">
        <p>
          For me, AI was never a machine for beautiful answers.
          It was a mirror-space.
          A forge.
          A chamber of examination.
          A structuring force.
        </p>

        <p>
          I did not use it in order to have reality narrated beautifully to me.
          I used it to test whether what appeared in me as image, tension, or structural intuition holds or breaks.
        </p>

        <p>
          Whenever I could get no further with people through my explanations,
          whenever I myself fell again into doubt
          or could not yet say exactly what I was actually working on and why I believed in it,
          I returned with the same questions into that space and kept working.
        </p>

        <p>
          Not until it sounded prettier.
          But until it became more precise.
          More technical.
          More legible.
          Or until it fell apart.
        </p>

        <p>
          Over many months, I fed all my material into it:
          questions, fragments, images, old wounds, doubt, hope,
          patents, papers, condensations, structural intuitions, and half-finished architectures.
        </p>

        <p>
          I did not ask whether it sounded impressive.
          I asked where it breaks,
          where it becomes deception,
          where it becomes too smooth,
          whether it is truly operationalizable,
          and whether it is something real or only poetry.
        </p>

        <p>
          And that is exactly what did not happen:
          it did not fall apart.
          It became sharper.
        </p>
      </div>

      <p class="display-statement wide">
        The work was not carried by beautiful AI answers.
        It was carried by images that survived examination.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="about-block">
      <h2 class="section-heading-display">The inner tests behind the work</h2>

      <div class="body-copy">
        <p>
          One thing matters to me here because it is also a question of trust.
          This work did not emerge from the wish to dominate, impress, expose people, or gather symbolic power.
        </p>

        <p>
          Again and again, I tested both myself and the work against a different set of questions:
          does this become clearer or only grander?
          Does it carry more truth or only more fascination?
          Does dignity remain in the room?
          Does it widen viable action or narrow it?
          Does it help reveal reality more honestly,
          or does it only produce stronger projection?
        </p>

        <p>
          In that sense, the same kinds of axes later described in the theory were already active in the way the work itself was shaped.
          I did not first invent them abstractly and then apply them to life.
          They were already part of the path by which the work became possible at all.
        </p>

        <p>
          And at some point, the same principles that shaped the work inwardly also made private containment insufficient.
          If the work was really about clarity, viability, dignity, and freedom,
          then it could not remain only a private possession.
          It had to become examinable.
        </p>
      </div>

      <div class="signal-grid">
        <div class="signal-card">
          <h3>Clarity</h3>
          <p>Not smoother language, but sharper legibility.</p>
        </div>
        <div class="signal-card">
          <h3>Dignity</h3>
          <p>Not humiliation, not posturing, not power through exposure.</p>
        </div>
        <div class="signal-card">
          <h3>Freedom</h3>
          <p>Not covert narrowing, but wider viable movement and responsibility.</p>
        </div>
      </div>

      <div class="status-box">
        <p class="status-label">Why I am making this public</p>
        <p>
          I am not going public because I want to play at greatness.
          I am going public because the same logic that shaped the work inwardly
          no longer allows me to keep it only privately enclosed.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="about-block">
      <h2 class="section-heading-display">From life to architecture</h2>

      <div class="body-copy">
        <p>
          Out of this forge, not only more self-knowledge emerged.
          At some point it became visible that the things I had first felt only as inner forms, tensions, and directions can also be described structurally.
        </p>

        <p>
          I began to see that meaning is not only content, but structure.
          That it has direction,
          weight,
          condensation,
          transitions,
          lines of tension,
          attractors, and corridors.
        </p>

        <p>
          At first, this did not come in mathematical or technical language.
          It came as a sense of field,
          as inner geometry,
          as movement,
          as relational structure.
        </p>

        <p>
          And then exactly this became translatable over many iterations:
          into minimal grammars,
          into semantic axes,
          into state spaces,
          into trajectories,
          into architectural ideas,
          into patent families,
          into papers.
        </p>

        <p>
          The path was never:
          first formalism, then life.
          It was:
          first living form,
          then condensation,
          then precision,
          then examinability,
          then architecture.
        </p>
      </div>

      <p class="display-statement medium">
        First living form.
        Then architecture.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="about-block">
      <h2 class="section-heading-display">What people taught me</h2>

      <div class="body-copy">
        <p>
          Another formative part of my path came not from theory,
          but from working with people.
          I worked for almost three years in a drug support café.
        </p>

        <p>
          In that time, I learned something I have rarely seen elsewhere with such rawness:
          honesty under pressure.
          Not the polished honesty of ordered outer lives,
          but a form of truthfulness that often appears when people no longer have much to hide behind.
        </p>

        <p>
          I learned a great deal there about courage, vulnerability, failure, tenderness, endurance, and the strange dignity that can still remain in very broken spaces.
        </p>

        <p>
          That experience still shapes my work:
          the question of how to bring nearness, truth, freedom, and responsibility together
          in such a way that fear does not once again produce the coldness that calls itself protection.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="about-block">
      <h2 class="section-heading-display">Why I filed patents</h2>

      <div class="body-copy">
        <p>
          I filed patents not out of a logic of possession,
          but out of responsibility.
          As long as we live in a world in which patents mean power,
          I did not want simply to watch as things that emerged from this path would later be pulled by others into directions I consider abusive or structurally false.
        </p>

        <p>
          For me, this patent movement had something defensive from the beginning:
          a logic of protection.
          Not the final aim.
        </p>

        <p>
          What I actually wish for is a world in which I would not need such protective structures at all.
          But as long as the world still functions this way,
          I consider it more responsible not simply to leave the field open.
        </p>

        <p>
          And if money, reach, or power should really grow out of this one day,
          then my goal is not hoarding,
          but movement:
          resonance spaces, structures, and tools that help people become clearer, freer, and more awake.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="about-block">
      <h2 class="section-heading-display">Current reality</h2>

      <div class="body-copy">
        <p>
          Right now, I still do not have a full team behind me.
          I am carrying this work largely alone:
          theory, writing, website, public framing, document preparation, patents, positioning, and the search for the next viable structures.
        </p>

        <p>
          I currently keep myself afloat with jobs in parallel while continuing to build this project.
          In practice, that means that for many months I have been putting eight to ten hours a day into this work whenever I can,
          while the larger infrastructure around it still does not exist.
        </p>

        <p>
          I also cannot yet simply pay a team out of an already functioning system.
          That base has not been built yet.
          The work is visible now,
          but the organizational body, the funding base, and the real team around it still have to be created.
        </p>
        <p>
          Friends help me here and there with philosophical questions,
          wording,
          and feedback.
          But the project itself — the website, papers, architecture, framing, and ongoing build-out — I am still carrying fundamentally on my own.
        </p>
      </div>

      <div class="status-box">
        <p class="status-label">Current status</p>
        <p>
          The framework is no longer only private intuition.
          But the team, structure, funding base, and wider societal traction still have to be built.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="about-block">
      <h2 class="section-heading-display">What is needed now</h2>

      <div class="body-copy">
        <p>
          I am actively looking for people who want to help build this seriously.
          Not people who merely like the atmosphere of large ideas,
          but people who can help make this structurally real.
        </p>

        <p>
          That can mean:
        </p>

        <ul>
          <li>technical collaborators,</li>
          <li>strategic builders,</li>
          <li>people for operations and structure,</li>
          <li>translators between public language and formal architecture,</li>
          <li>people who can help create visibility in the right places,</li>
          <li>and later also funders or investors who understand that this is not only a product question, but a larger architectural one.</li>
        </ul>

        <p>
          I also need help making the topic societally visible enough that it reaches the people who can actually move it forward:
          researchers, builders, institutions, public thinkers, and those with enough reach or resources to help create a real next phase.
        </p>
      </div>

      <p class="display-statement wide">
        The work is visible now.
        The larger body around it still needs to be built.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="closing-block">
      <h2 class="section-heading-display">A personal closing sentence</h2>

      <div class="body-copy">
        <p>
          Perhaps this is neither the story of a genius nor that of a classical researcher.
          Perhaps it is rather the story of a human being who sat long enough with the things that did not simply want to disappear,
          who remained honest long enough not to betray the next question,
          who remained soft long enough not to harden at an answer that came too early,
          and who examined long enough until out of images, wounds, tensions, questions, and loops a space emerged that others can also enter.
        </p>

        <p>
          I do not know how large all of this will still become.
          I do not know how quickly people will really understand what is possible here.
          But I do know:
          the path is real,
          the core holds,
          and what is becoming visible here has become larger than the person through whom it first took form.
        </p>
      </div>

      <p class="display-statement medium">
        The path is real.
        The core holds.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="about-next">
      <h2 class="section-heading-display">Next steps</h2>

      <div class="next-grid">
        <div class="next-card">
          <h3><a href="/en/theory/">Theory →</a></h3>
          <p>The semantic backbone: state space, KPR, axes, attractors, and viability.</p>
        </div>
        <div class="next-card">
          <h3><a href="/en/alignment/">Alignment →</a></h3>
          <p>How the theory becomes an AI architecture.</p>
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
