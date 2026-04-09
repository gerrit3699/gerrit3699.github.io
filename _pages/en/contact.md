---
layout: default
title: "Contact & Support"
permalink: /en/contact/
lang: en
description: "Contact Gerrit Klawitter, Semantic Gravitation, support, collaboration, and PayPal."
translation_url_de: /de/kontakt/
---

<style>
  html {
    scroll-behavior: smooth;
  }

  .contact-page {
    --contact-text: rgba(255,255,255,0.96);
    --contact-soft: rgba(255,255,255,0.82);
    --contact-faint: rgba(255,255,255,0.62);
    --contact-line: rgba(255,255,255,0.10);
    --contact-line-strong: rgba(255,255,255,0.16);
  }

  .contact-page h1,
  .contact-page h2,
  .contact-page h3,
  .contact-page strong,
  .contact-page a {
    color: #fff;
  }

  .contact-page p,
  .contact-page li {
    color: var(--contact-text);
  }

  .contact-page .section-shell {
    padding-top: 2.9rem;
    padding-bottom: 2.9rem;
  }

  .contact-page .section-shell-tight {
    padding-top: 2.2rem;
    padding-bottom: 2.2rem;
  }

  .contact-page .contact-intro,
  .contact-page .contact-block,
  .contact-page .contact-next {
    max-width: 1080px;
    margin: 0 auto;
  }

  .contact-page .contact-intro,
  .contact-page .body-copy,
  .contact-page .closing-block,
  .contact-page .contact-next {
    text-align: center;
  }

  .contact-page .contact-kicker,
  .contact-page .status-label {
    margin: 0 0 0.7rem;
    font-size: 0.88rem;
    letter-spacing: 0.16em;
    text-transform: uppercase;
    color: var(--contact-faint);
  }

  .contact-page .contact-display {
    margin: 0 auto 1.15rem;
    max-width: 11ch;
    font-size: clamp(2.5rem, 6vw, 5rem);
    line-height: 0.94;
    letter-spacing: -0.05em;
    font-weight: 650;
    text-wrap: balance;
  }

  .contact-page .contact-sublead {
    max-width: 58rem;
    margin: 0 auto 1.2rem;
    font-size: clamp(1.08rem, 2vw, 1.4rem);
    line-height: 1.62;
    text-wrap: balance;
  }

  .contact-page .claim-grid,
  .contact-page .support-grid,
  .contact-page .next-grid {
    display: grid;
    gap: 1rem;
  }

  .contact-page .claim-grid,
  .contact-page .support-grid {
    grid-template-columns: repeat(3, minmax(0, 1fr));
    max-width: 1080px;
    margin: 1.9rem auto 0;
  }

  .contact-page .next-grid {
    grid-template-columns: repeat(4, minmax(0, 1fr));
    max-width: 1080px;
    margin: 1.8rem auto 0;
  }

  .contact-page .claim-card,
  .contact-page .support-card,
  .contact-page .next-card,
  .contact-page .status-box,
  .contact-page .contact-card {
    border: 1px solid var(--contact-line);
    border-radius: 22px;
    background:
      linear-gradient(180deg, rgba(8,10,14,0.68), rgba(5,7,11,0.82)),
      url("/assets/images/design/fog.jpg.PNG") center center / cover no-repeat;
    box-shadow:
      0 18px 48px rgba(0,0,0,0.18),
      inset 0 1px 0 rgba(255,255,255,0.03);
  }

  .contact-page .claim-card,
  .contact-page .support-card,
  .contact-page .next-card,
  .contact-page .contact-card {
    padding: 1.18rem 1rem 1.08rem;
    text-align: center;
  }

  .contact-page .claim-card h3,
  .contact-page .support-card h3,
  .contact-page .next-card h3,
  .contact-page .contact-card h3 {
    margin: 0 0 0.35rem;
    font-size: 1.18rem;
    line-height: 1.08;
    letter-spacing: -0.03em;
  }

  .contact-page .claim-card p,
  .contact-page .support-card p,
  .contact-page .next-card p,
  .contact-page .contact-card p {
    margin: 0;
    font-size: 0.98rem;
    line-height: 1.56;
    color: var(--contact-soft);
  }

  .contact-page .claim-card {
    display: block;
    text-decoration: none;
    transition:
      transform 0.18s ease,
      border-color 0.18s ease,
      background-color 0.18s ease;
  }

  .contact-page .claim-card:hover {
    transform: translateY(-2px);
    border-color: var(--contact-line-strong);
  }

  .contact-page .section-heading-display {
    margin: 0 auto 1.3rem;
    max-width: 14ch;
    text-align: center;
    font-size: clamp(2.05rem, 4.8vw, 3.7rem);
    line-height: 0.98;
    letter-spacing: -0.045em;
    text-wrap: balance;
  }

  .contact-page .body-copy {
    max-width: 940px;
    margin: 0 auto;
  }

  .contact-page .body-copy p {
    max-width: 47em;
    margin: 0.95rem auto 0;
    font-size: 1.1rem;
    line-height: 1.78;
    letter-spacing: -0.01em;
  }

  .contact-page .body-copy ul,
  .contact-page .body-copy ol {
    max-width: 42em;
    margin: 1.15rem auto;
    text-align: left;
    padding-left: 1.15rem;
  }

  .contact-page .body-copy li {
    margin-bottom: 0.45rem;
  }

  .contact-page .display-statement {
    max-width: 24ch;
    margin: 1.9rem auto;
    text-align: center;
    font-size: clamp(1.9rem, 3.6vw, 3rem);
    line-height: 1.03;
    letter-spacing: -0.045em;
    font-weight: 650;
    text-wrap: balance;
  }

  .contact-page .display-statement.wide { max-width: 30ch; }
  .contact-page .display-statement.medium { max-width: 22ch; }
  .contact-page .display-statement.narrow { max-width: 12ch; }

  .contact-page .status-box {
    max-width: 920px;
    margin: 2rem auto 0;
    padding: 1.2rem 1.15rem;
    text-align: center;
  }

  .contact-page .status-box p {
    margin: 0;
    font-size: clamp(1.18rem, 2.2vw, 1.7rem);
    line-height: 1.38;
    text-wrap: balance;
  }

  .contact-page .contact-links {
    display: grid;
    gap: 1rem;
    max-width: 780px;
    margin: 2rem auto 0;
  }

  .contact-page .contact-link {
    display: block;
    padding: 1rem 1.1rem;
    border-radius: 18px;
    border: 1px solid var(--contact-line);
    background: rgba(255,255,255,0.04);
    text-decoration: none;
    font-size: 1.06rem;
    line-height: 1.45;
  }

  .contact-page .support-link {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 52px;
    padding: 0.95rem 1.25rem;
    border-radius: 999px;
    border: 1px solid var(--contact-line);
    background: rgba(255,255,255,0.06);
    text-decoration: none;
    font-size: 1.02rem;
    line-height: 1.2;
    margin-top: 1rem;
  }

  .contact-page .next-card a {
    color: #fff;
  }

  @media (max-width: 980px) {
    .contact-page .claim-grid,
    .contact-page .support-grid,
    .contact-page .next-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="contact-page">

  <section class="section-shell section-shell-tight">
    <div class="contact-intro">
      <p class="contact-kicker">Contact & Support</p>
      <h1 class="contact-display">Get in touch.</h1>
      <p class="contact-sublead">
        For contact, resonance, collaboration, support, and serious offers to help build
        Semantic Gravitation into something structurally real.
      </p>

      <div class="claim-grid">
        <a class="claim-card" href="#contact">
          <h3>Contact</h3>
          <p>Write if the work reached you, if you have a serious question, or if you want to connect.</p>
        </a>
        <a class="claim-card" href="#support">
          <h3>Support</h3>
          <p>Financial support makes a very real difference in this phase.</p>
        </a>
        <a class="claim-card" href="#help-build">
          <h3>Help build</h3>
          <p>Contacts, reach, structure, heart, strategy, media, and technical collaboration are all relevant.</p>
        </a>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="contact-block">
      <h2 class="section-heading-display">Current situation</h2>

      <div class="body-copy">
        <p>
          Semantic Gravitation is still being built under very real conditions.
          I am currently working on it largely on my own:
          website, papers, architecture, writing, public framing, downloads, positioning, and the next structural steps.
        </p>

        <p>
          Friends help me here and there with philosophical questions,
          wording,
          and feedback.
          But the project itself I am still carrying fundamentally alone.
        </p>

        <p>
          At the same time, I currently still keep myself afloat with jobs.
          This project is not yet backed by a real team,
          not by stable funding,
          and not by a larger institutional structure.
          Much of it has been built through sustained work over many months,
          often with eight to ten hours a day going into it whenever possible.
        </p>
      </div>

      <p class="display-statement wide">
        The work is real.
        The structure around it still has to be built.
      </p>

      <div class="status-box">
        <p class="status-label">What that means in practice</p>
        <p>
          Right now, support, contacts, funding, visibility, and serious collaboration do not help abstractly.
          They help very concretely.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell" id="contact">
    <div class="contact-block">
      <h2 class="section-heading-display">Contact</h2>

      <div class="body-copy">
        <p>
          If the work on <strong>semanticgravitation.org</strong> speaks to you,
          if you feel resonance,
          if you want to offer serious feedback,
          bring in contacts,
          support the project,
          or suggest a way you could help,
          you can reach out here.
        </p>
      </div>

      <div class="contact-links">
        <a class="contact-link" href="mailto:contact@semanticgravitation.org">
          <strong>Email:</strong> contact@semanticgravitation.org
        </a>

        <a class="contact-link" href="https://instagram.com/semanticgravitation" target="_blank" rel="noopener">
          <strong>Instagram:</strong> @semanticgravitation
        </a>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell" id="help-build">
    <div class="contact-block">
      <h2 class="section-heading-display">How you can help</h2>

      <div class="support-grid">
        <div class="support-card">
          <h3>Contacts & reach</h3>
          <p>Introduce the work to the right people, networks, institutions, builders, or public thinkers.</p>
        </div>
        <div class="support-card">
          <h3>Building & structure</h3>
          <p>Help with organization, website, media, technical build-out, design, public communication, or operations.</p>
        </div>
        <div class="support-card">
          <h3>Funding & support</h3>
          <p>Help create the financial room in which this can become more continuous, public, and buildable.</p>
        </div>
      </div>

      <div class="body-copy">
        <p>
          You do not need a pre-defined role in order to write.
          If you feel seriously addressed by this work,
          you can also simply say what you can bring.
        </p>

        <p>
          I do not want to force everything immediately into rigid boxes.
          Over time, I want to build a field in which clearer roles, responsibilities, and forms of collaboration can emerge.
          But right now, part of what matters is simply making the right contact visible at all.
        </p>
      </div>

      <p class="display-statement medium">
        If you feel called,
        write.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell" id="support">
    <div class="contact-block">
      <h2 class="section-heading-display">Support</h2>

      <div class="body-copy">
        <p>
          If you would like to support my work directly,
          you can do so here.
        </p>

        <p>
          Your support helps make the time, energy, and infrastructure for this project more viable:
          for research, writing, publication, website, public communication,
          further development of the architecture,
          and the long-term building of Semantic Gravitation.
        </p>

        <p>
          Especially in this phase, support makes a real difference.
          It reduces pressure,
          creates room,
          and makes it more realistic to bring this work into the world
          not only alongside everything else,
          but with more continuity, depth, and reach.
        </p>

        <p>
          I will continue this work either way.
          But if this project touches you,
          if you consider it important,
          or if you want to help something viable grow from it,
          your contribution helps in a very concrete way right now.
        </p>
      </div>

      <a class="support-link" href="https://paypal.me/semanticgravitation" target="_blank" rel="noopener">
        Support my work
      </a>

      <div class="body-copy">
        <p>
          <a href="https://paypal.me/semanticgravitation" target="_blank" rel="noopener">paypal.me/semanticgravitation</a>
        </p>

        <p>
          At the moment, support is best understood as a voluntary contribution
          to enabling and further developing this work.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="contact-block">
      <h2 class="section-heading-display">Before you write</h2>

      <div class="body-copy">
        <p>
          I appreciate serious messages.
          What I currently cannot do, and also do not want to do,
          is explain from the beginning again and again in individual conversations
          what Semantic Gravitation is,
          why it might work,
          or how every building block is derived in detail.
        </p>

        <p>
          If you really want to understand what this is about,
          please first use the materials on the site:
          especially the Theory page,
          the Technical Sources,
          the Downloads,
          and the alignment material.
        </p>

        <p>
          My suggestion is:
          take your real question,
          load the documents into an AI of your choice,
          work your way into the material yourself,
          and examine the point that truly interests, irritates, or calls you.
        </p>

        <p>
          Do not believe too quickly.
          Do not reject too quickly.
          But ask precisely,
          examine carefully,
          and make your own short-circuit the starting point of the next better question.
        </p>
      </div>

      <div class="status-box">
        <p class="status-label">A good message helps</p>
        <p>
          What reached you?
          What matters to you?
          What can you contribute, ask, connect, or help set in motion?
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="closing-block">
      <h2 class="section-heading-display">Note</h2>

      <div class="body-copy">
        <p>
          I read messages as well as I can.
          Especially in more intensive phases, a reply may take some time.
        </p>

        <p>
          Clear, concrete, and honest messages help most.
          Serious resonance is welcome.
          Serious help is welcome.
          Serious support is welcome.
        </p>
      </div>
    </div>
  </section>

</div>
