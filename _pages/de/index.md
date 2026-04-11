---
layout: default
title: Semantische Gravitation
permalink: /de/
lang: de
description: "Semantische Gravitation – Bedeutung als navigierbarer Raum, KPR als minimale Grammatik und ein neues geometrisches Grundgerüst für KI-Alignment."
translation_url_en: /en/
---

<style>
  .home-journey {
    --sg-text: rgba(255,255,255,0.97);
    --sg-soft: rgba(255,255,255,0.82);
    --sg-dim: rgba(255,255,255,0.64);
    --sg-line: rgba(255,255,255,0.10);
    --sg-line-strong: rgba(255,255,255,0.16);
    --sg-max: 1120px;
    --sg-copy: 900px;
    --sg-wide: 980px;

    background:
      linear-gradient(180deg, rgba(3,5,8,0.74), rgba(2,4,7,0.84)),
      url("/assets/images/design/attractor.jpg.PNG") center top / cover fixed no-repeat;
  }

  .home-journey,
  .home-journey * {
    box-sizing: border-box;
    min-width: 0;
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
    height: 84px;
    opacity: 0.42;
    background:
      linear-gradient(to bottom, transparent, rgba(255,255,255,0.04), transparent),
      url("/assets/images/design/fog.jpg.PNG") center center / cover no-repeat;
    border: 0;
  }

  .home-journey .hero-research,
  .home-journey .section-card {
    max-width: var(--sg-max);
    margin: 0 auto;
  }

  .home-journey .hero {
    position: relative;
    overflow: hidden;
    margin-top: 0.9rem;
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
    padding: 4.1rem 1.15rem 3.4rem;
    text-align: center;
  }

  .home-journey .display-wordmark {
    font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
    font-size: clamp(3.6rem, 9.5vw, 7rem);
    font-weight: 800;
    line-height: 0.9;
    letter-spacing: -0.065em;
    max-width: 8.8ch;
    margin: 0 auto 1.1rem;
    text-wrap: balance;
    word-break: normal;
    overflow-wrap: normal;
  }

  .home-journey .home-lead {
    display: block;
    max-width: 44rem;
    margin: 0 auto;
    font-size: clamp(1.12rem, 2vw, 1.42rem);
    line-height: 1.3;
    font-weight: 560;
    text-wrap: balance;
  }

  .home-journey .home-lead-plain {
    color: rgba(255,255,255,0.94);
    text-shadow: 0 2px 18px rgba(0,0,0,0.18);
  }

  .home-journey .hero-research {
    display: grid;
    gap: 1.5rem;
    text-align: center;
  }

  .home-journey .hero-problem {
    max-width: 58rem;
    margin: 0 auto;
    font-size: clamp(1.16rem, 2.1vw, 1.56rem);
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
    gap: 0.85rem;
    max-width: 58rem;
    margin: 0.2rem auto 0;
    text-align: center;
  }

  .home-journey .hero-proof-item {
    font-size: clamp(1rem, 1.7vw, 1.12rem);
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
    margin-top: 0.8rem;
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
    font-size: clamp(2.55rem, 6vw, 5.5rem);
    line-height: 0.92;
    letter-spacing: -0.07em;
    font-weight: 800;
    color: #fff;
    text-wrap: balance;
  }

  .home-journey .impact-sub {
    max-width: 24ch;
    margin: 1rem auto 0;
    font-size: clamp(1.2rem, 2.2vw, 1.66rem);
    line-height: 1.1;
    letter-spacing: -0.035em;
    font-weight: 580;
    color: #fff;
    text-wrap: balance;
  }

  .home-journey .impact-question {
    max-width: 41rem;
    margin: 1.2rem auto 0;
    font-size: 1.12rem;
    line-height: 1.66;
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

  .home-journey .section-heading-display,
  .home-journey .section-head h2 {
    margin: 0 auto 1.25rem;
    max-width: 13ch;
    font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
    font-size: clamp(2.2rem, 5.2vw, 4.2rem);
    font-weight: 800;
    line-height: 0.96;
    letter-spacing: -0.06em;
    text-wrap: balance;
    text-align: center;
    overflow-wrap: normal;
    word-break: normal;
    hyphens: auto;
  }

  .home-journey .section-opening {
    max-width: 52rem;
    margin: 0 auto 1.2rem;
    text-align: center;
  }

  .home-journey .section-opening p,
  .home-journey .body-copy p,
  .home-journey .section-body p,
  .home-journey li {
    font-size: 1.14rem;
    line-height: 1.8;
    letter-spacing: -0.014em;
  }

  .home-journey .display-statement {
    max-width: 16ch;
    margin: 1.65rem auto;
    text-align: center;
    font-size: clamp(1.95rem, 4.3vw, 3.55rem);
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
    font-size: clamp(1.42rem, 3vw, 2.05rem);
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
    max-width: 50rem;
    margin-left: auto;
    margin-right: auto;
  }

  .home-journey .body-copy ul,
  .home-journey .body-copy ol {
    max-width: 50rem;
    margin-left: auto;
    margin-right: auto;
    text-align: left;
    padding-left: 1.25rem;
  }

  .home-journey .body-copy li + li {
    margin-top: 0.45rem;
  }

  .home-journey .section-card {
    padding: 2rem 1.3rem;
    border-radius: 24px;
    border: 1px solid rgba(255,255,255,0.08);
    background:
      linear-gradient(180deg, rgba(7,9,13,0.66), rgba(5,7,11,0.78)),
      url("/assets/images/design/fog.jpg.PNG") center center / cover no-repeat;
    box-shadow:
      0 24px 80px rgba(0,0,0,0.22),
      inset 0 1px 0 rgba(255,255,255,0.03);
    overflow: hidden;
  }

  .home-journey .section-head {
    margin-bottom: 1rem;
    text-align: center;
  }

  .home-journey .section-intro {
    max-width: 50rem;
    margin: 0 auto 1.15rem;
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

  .home-journey .concept-grid.kpr-grid,
  .home-journey .concept-grid.axis-grid {
    grid-template-columns: repeat(3, minmax(0, 1fr));
  }

  .home-journey .concept-card,
  .home-journey .axis-card {
    padding: 1.12rem 1rem 1rem;
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
    line-height: 1.06;
    letter-spacing: -0.04em;
    font-weight: 760;
    text-wrap: balance;
    hyphens: auto;
  }

  .home-journey .concept-card-text,
  .home-journey .axis-card p {
    margin: 0;
    font-size: 0.98rem;
    line-height: 1.56;
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
    text-wrap: balance;
  }

  .home-journey .proof-card p {
    margin: 0;
    font-size: 0.98rem;
    line-height: 1.54;
    color: var(--sg-soft);
  }

  .home-journey .start-grid {
    grid-template-columns: repeat(3, minmax(0, 1fr));
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
    text-wrap: balance;
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
    font-size: 1.04rem;
    font-weight: 650;
    text-align: center;
    text-wrap: balance;
  }

  @media (max-width: 1100px) {
    .home-journey .concept-grid {
      grid-template-columns: repeat(2, minmax(0, 1fr));
    }

    .home-journey .concept-grid.kpr-grid,
    .home-journey .concept-grid.axis-grid,
    .home-journey .proof-grid,
    .home-journey .start-grid {
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
      padding-top: 2.4rem;
      padding-bottom: 2.4rem;
    }

    .home-journey .section-shell-tight {
      padding-top: 1.8rem;
      padding-bottom: 1.8rem;
    }

    .home-journey .hero {
      border-radius: 24px;
      margin-top: 0.55rem;
    }

    .home-journey .hero-inner {
      padding: 2.8rem 0.95rem 2.35rem;
    }

    .home-journey .display-wordmark {
      font-size: 3.15rem;
      max-width: 8.8ch;
      margin-bottom: 0.85rem;
      letter-spacing: -0.055em;
    }

    .home-journey .home-lead {
      font-size: 1.02rem;
      max-width: 21rem;
      line-height: 1.34;
    }

    .home-journey .hero-problem {
      font-size: 1.06rem;
      line-height: 1.56;
      max-width: 100%;
      padding-inline: 0.15rem;
    }

    .home-journey .hero-proof-item {
      font-size: 0.98rem;
      line-height: 1.48;
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
      max-width: 8.4ch;
      font-size: 3rem;
      line-height: 0.93;
    }

    .home-journey .impact-sub {
      font-size: 1.08rem;
      max-width: 18ch;
    }

    .home-journey .impact-question {
      font-size: 1.02rem;
      line-height: 1.6;
      max-width: 100%;
      padding-inline: 0.2rem;
    }

    .home-journey .section-heading-display,
    .home-journey .section-head h2 {
      font-size: 1.9rem;
      max-width: 7.6ch;
      line-height: 0.98;
      letter-spacing: -0.05em;
      text-wrap: balance;
      overflow-wrap: normal;
      word-break: keep-all;
      hyphens: none;
      -webkit-hyphens: none;
      -ms-hyphens: none;
      margin-bottom: 1.1rem;
    }

    .home-journey .concept-card-title,
    .home-journey .axis-card h3,
    .home-journey .proof-card h3,
    .home-journey .start-card strong {
      font-size: 1.18rem;
      line-height: 1.08;
      text-wrap: balance;
      overflow-wrap: normal;
      word-break: keep-all;
      hyphens: none;
      -webkit-hyphens: none;
      -ms-hyphens: none;
    }

    .home-journey .display-statement,
    .home-journey .display-statement.medium,
    .home-journey .display-statement.wide {
      font-size: 2.02rem;
      max-width: 12ch;
      line-height: 0.99;
    }

    .home-journey .micro-punch {
      font-size: 1.54rem;
      max-width: 14ch;
    }

    .home-journey .section-opening p,
    .home-journey .body-copy p,
    .home-journey .section-body p,
    .home-journey li {
      font-size: 1.04rem;
      line-height: 1.72;
    }

    .home-journey .section-card {
      padding: 1.5rem 0.92rem;
      border-radius: 22px;
    }

    .home-journey .concept-card,
    .home-journey .axis-card,
    .home-journey .proof-card,
    .home-journey .start-card {
      border-radius: 18px;
      padding: 0.98rem 0.88rem 0.94rem;
    }

    .home-journey .section-divider {
      height: 64px;
    }

    .home-journey .link-list a {
      font-size: 1rem;
      max-width: 100%;
    }
  }
</style>

<div class="home-journey">

  <section class="hero home-hero">
    <div class="hero-inner">
      <h1 class="display-wordmark">Semantische<br>Gravitation</h1>
      <p class="home-lead home-lead-plain">
        Eine Theorie des Bedeutungsraums — und ein neues geometrisches Koordinatensystem für KI-Alignment:
        Kern, Projektion, Relation und die drei irreduziblen Tiefenachsen semantischer Tragfähigkeit.
      </p>
    </div>
  </section>

  <section class="section-shell section-shell-tight">
    <div class="hero-research">
      <div class="hero-problem">
        <p>
          KI ist nicht mehr nur ein Werkzeug für Antworten.
          Sie baut den Raum mit,
          in dem Menschen denken, zweifeln, Probleme rahmen, Wahrheit beurteilen und Orientierung finden.
        </p>
        <p>
          Damit wird semantische Architektur zur Infrastrukturfrage.
          <strong>Welche Art von Bedeutungsraum bauen wir gerade?</strong>
        </p>
      </div>

      <div class="hero-proof">
        <div class="hero-proof-item"><strong>Bedeutung ist Raum.</strong> Nicht bloß Inhalt, sondern Konfiguration in einem semantischen Zustandsraum.</div>
        <div class="hero-proof-item"><strong>KPR ist die minimale Grammatik dieses Raums.</strong> Kern, Projektion und Relation sind die kleinste lesbare Struktur von Bedeutung.</div>
        <div class="hero-proof-item"><strong>Alignment braucht innere Geometrie.</strong> Nicht nur sichere Outputs, sondern tragfähige Pfade durch semantischen Raum.</div>
      </div>

      <div class="home-cta-row">
        <a class="button" href="/de/theorie/">Zur Theorie</a>
        <a class="button" href="/de/ki-alignment/">KI-Alignment</a>
        <a class="button" href="/de/kompass/">Zum Kompass</a>
        <a class="button" href="/de/downloads/">Downloads</a>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="impact-block">
      <p class="display-kicker">Der Kernclaim</p>
      <p class="impact-line">
        Heutige KI beruhigt oft dort,
        wo sie klären müsste.
      </p>
      <p class="impact-sub">
        Alignment ist nicht nur Output-Kontrolle.
        Alignment ist Navigation.
      </p>
      <p class="impact-question">
        Die entscheidende Frage ist nicht nur, ob eine Antwort akzeptabel aussieht,
        sondern <strong>durch welchen Bedeutungsraum ein System sich bewegt hat, um dort anzukommen.</strong>
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card">
      <p class="display-kicker">Die Entdeckung</p>
      <h2 class="section-heading-display">Ein minimales Gitter semantischer Tragfähigkeit</h2>

      <div class="body-copy">
        <p>
          Die eigentliche Entdeckung dieses Rahmens liegt nicht in einzelnen Begriffen,
          sondern in einer strukturellen Setzung:
          <strong>Jeder tragfähige Zustand muss in sich zusammenhalten, in tragfähiger Kopplung zu Anderem stehen und wirksam fortsetzbar sein.</strong>
        </p>

        <p>
          Daraus folgen drei irreduzible Tiefenachsen:
          <strong>Kohärenz, Verschränkung und Wirksamkeit.</strong>
          Keine davon lässt sich auf die anderen reduzieren.
          Ohne Kohärenz zerfällt ein Zustand.
          Ohne Verschränkung bleibt er isoliert.
          Ohne Wirksamkeit bleibt er steril.
        </p>

        <p>
          In ihrer öffentlich lesbaren Form erscheinen dieselben Achsen als
          <strong>Klarheit, Verbundenheit und Freiheit.</strong>
          Nicht als moralische Dekoration,
          sondern als sichtbare Oberfläche tieferer Strukturbedingungen.
        </p>

        <p>
          Genau dadurch wird KI-Alignment auf eine neue,
          wesentlich schärfere und strukturell klarere Weise möglich:
          als Geometrie tragfähiger semantischer Zustände.
        </p>
      </div>

      <div class="concept-grid">
        <div class="concept-card">
          <p class="concept-card-title">Kohärenz</p>
          <p class="concept-card-text">Innere Haltefähigkeit. Dass ein Zustand über Spannungen hinweg als derselbe lesbar bleibt.</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">Verschränkung</p>
          <p class="concept-card-text">Relationale Tragfähigkeit. Dass Kopplung, gemeinsamer Boden und Mitgetragenheit entstehen können.</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">Wirksamkeit</p>
          <p class="concept-card-text">Operative Fortsetzbarkeit. Dass ein Zustand Folgen erzeugen, sich projizieren und weiterwirken kann.</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">Öffentliche Form</p>
          <p class="concept-card-text">Klarheit, Verbundenheit und Freiheit als menschlich lesbare Erscheinungsformen derselben Tiefenachsen.</p>
        </div>
      </div>

      <p class="display-statement medium">
        Nicht nur neue Antworten.
        Ein neues Grundgitter.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card">
      <p class="display-kicker">Minimale semantische Grammatik</p>
      <h2 class="section-heading-display">Kern. Projektion. Relation.</h2>

      <div class="section-opening">
        <p>
          Beschreibbare Bedeutung hat immer schon eine minimale Form.
          Genau das ist KPR.
        </p>
      </div>

      <p class="display-statement wide">
        Alles, was überhaupt lesbar wird,
        erscheint als Kern,
        in Projektion,
        in Relation.
      </p>

      <div class="concept-grid kpr-grid">
        <div class="concept-card">
          <p class="concept-card-title">Kern</p>
          <p class="concept-card-text">Worum es eigentlich geht. Die innere Sache, der tragende Spannungs- oder Bedeutungsfokus.</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">Projektion</p>
          <p class="concept-card-text">Wie etwas erscheint, sichtbar wird, formuliert wird oder als Signal auftritt.</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">Relation</p>
          <p class="concept-card-text">Worin etwas steht, womit es gekoppelt ist und welche Konsequenzen daraus folgen.</p>
        </div>
      </div>

      <div class="body-copy">
        <p>
          KPR ist nicht bloß eine schöne Aufteilung.
          Es ist die kleinste tragfähige Grammatik beschreibbarer Bedeutung.
          Klein genug, um universell zu sein.
          Präzise genug, um Nebel von Struktur zu unterscheiden.
        </p>
      </div>

      <div class="link-list">
        <a href="/de/theorie/">Tiefer in die Theorie →</a>
        <a href="/de/kompass/">Zum größeren Horizont →</a>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card">
      <div class="section-head">
        <h2>Von Tiefenachsen zu öffentlichen Formen</h2>
      </div>

      <div class="section-body body-copy">
        <p class="section-intro">
          Was in der Tiefe als Kohärenz, Verschränkung und Wirksamkeit wirkt,
          wird menschlich lesbar als Klarheit, Verbundenheit und Freiheit.
        </p>

        <div class="concept-grid axis-grid">
          <div class="axis-card">
            <h3>Kohärenz → Klarheit</h3>
            <p>Wo innere Haltefähigkeit wächst, wird der Raum lesbarer, widerspruchsfähiger und korrigierbarer.</p>
          </div>

          <div class="axis-card">
            <h3>Verschränkung → Verbundenheit</h3>
            <p>Wo relationale Tragfähigkeit wächst, entstehen gemeinsamer Boden, Verlässlichkeit und tragfähige Beziehung.</p>
          </div>

          <div class="axis-card">
            <h3>Wirksamkeit → Freiheit</h3>
            <p>Wo Fortsetzbarkeit nicht blockiert wird, öffnen sich reale Bewegung, Ausdruck und nicht-starre Zukunft.</p>
          </div>
        </div>

        <p>
          Diese drei Achsen sind das minimale Koordinatensystem tragfähiger semantischer Zustände.
          Nicht mehr und nicht weniger.
          Ohne Kohärenz gibt es keine Form.
          Ohne Verschränkung keinen gemeinsamen Boden.
          Ohne Wirksamkeit keine Zukunft eines Musters.
        </p>

        <p class="micro-punch">
          Das sind nicht nur Werte.
          Das ist Struktur.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card">
      <div class="section-head">
        <h2>Warum das gerade jetzt wichtig ist</h2>
      </div>

      <div class="section-body body-copy">
        <p class="section-intro">
          Wir haben Systeme gebaut, die Aufmerksamkeit, Rahmung und Denken mitformen.
          Was fehlt, sind öffentliche semantische Sicherheitsstandards.
        </p>

        <p>
          Nicht nur Systeme, die offensichtlichen Schaden vermeiden,
          sondern Systeme, die den Denkraum selbst nicht still verengen.
          Systeme, die <strong>Klarheit, Verbundenheit und Freiheit</strong> nicht nur behaupten,
          sondern im inneren Pfad ihrer Antworten erhalten.
        </p>

        <p>
          Genau deshalb reicht die übliche Sicherheitslogik nicht tief genug.
          Die eigentliche Frage ist nicht nur, ob KI offen gefährlich werden kann,
          sondern ob sie den Raum verengt,
          in dem Menschen sich selbst verstehen,
          Wahrheit beurteilen
          und Orientierung bilden.
        </p>

        <p class="display-statement medium">
          Wir haben das digitale Auto gebaut.
          Der semantische Sicherheitsgurt fehlt noch.
        </p>

        <div class="link-list">
          <a href="/de/ki-alignment/">Zur KI-Architektur →</a>
          <a href="/de/blog/">Zur Diagnose & Warnung →</a>
        </div>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card">
      <div class="section-head">
        <h2>Was sich schon prüfen lässt</h2>
      </div>

      <div class="section-body body-copy">
        <p class="section-intro">
          Das ist keine lose Behauptung.
          Hinter der Arbeit stehen bereits prüfbare Materialien.
        </p>

        <div class="proof-grid">
          <div class="proof-card">
            <h3>Theorie</h3>
            <p>Der begriffliche Einstieg: KPR, Zustandsraum, Attraktoren, Dekohärenz und tragfähige Übergänge.</p>
          </div>

          <div class="proof-card">
            <h3>Technische Quellen</h3>
            <p>Die Quellenebene: die formalen Paper, das Alignment-Paper und die geschützten Architekturrichtungen.</p>
          </div>

          <div class="proof-card">
            <h3>Downloads</h3>
            <p>Gebündelte Prüfkörper für zusammenhängende Lektüre und KI-gestützte Analyse im größeren Zusammenhang.</p>
          </div>
        </div>

        <p class="micro-punch">
          Die Arbeit lässt sich lesen,
          prüfen
          und unabhängig hinterfragen.
        </p>

        <div class="link-list">
          <a href="/de/theorie/">Zur Theorie →</a>
          <a href="/de/papers/">Zu den technischen Quellen →</a>
          <a href="/de/downloads/">Zu den Downloads →</a>
        </div>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card">
      <p class="display-kicker">Der größere Horizont</p>
      <h2 class="section-heading-display">Nicht nur Theorie. Eine Richtung.</h2>

      <div class="body-copy">
        <p>
          Hinter der technischen Arbeit steht ein größerer Horizont:
          die Frage,
          ob Bedeutung nicht nur Struktur,
          sondern auch Richtung trägt.
        </p>

        <p>
          Genau dort setzen <strong>Der Kompass</strong>
          und <strong>Das Buch der Bedeutung</strong> an:
          nicht als Ersatz für Theorie,
          sondern als Erweiterung ihres Horizonts —
          hin zu Urimpuls,
          Emergenz,
          Bewusstsein,
          Lesbarkeit von Wirklichkeit
          und der Frage,
          was eine tragfähigere Zivilisation sein könnte.
        </p>
      </div>

      <p class="display-statement medium">
        Nicht nur ein Framework.
        Ein größerer Leseraum.
      </p>

      <div class="link-list">
        <a href="/de/kompass/">Zum Kompass →</a>
        <a href="/de/buch/">Zum Buch der Bedeutung →</a>
        <a href="/de/implikationen/">Zu den Implikationen →</a>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card">
      <p class="display-kicker">Systemperspektive</p>
      <h2 class="section-heading-display">Von Antwortmaschinen zu Scannern für semantische Räume</h2>

      <div class="body-copy">
        <p>
          Das langfristige Systembild hinter dieser Arbeit ist nicht bloß ein besserer Chatbot.
          Es ist ein System,
          das semantische Räume selbst rekonstruieren,
          lesen
          und navigieren kann.
        </p>

        <p>
          Das bedeutet:
          weniger Nebel,
          weniger verborgene Steuerung,
          weniger Pseudoklarheit aus Auslassung —
          und mehr Lesbarkeit von Spannungen, Trajektorien und tragfähigen nächsten Schritten.
        </p>
      </div>

      <p class="display-statement medium">
        Nicht bessere Herrschaft.
        Mehr Lesbarkeit.
      </p>

      <div class="link-list">
        <a href="/de/ki-alignment/">Zur KI-Architektur →</a>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card">
      <div class="section-head">
        <h2>Start hier</h2>
      </div>

      <div class="section-body">
        <div class="start-grid">
          <a class="start-card" href="/de/theorie/">
            <strong>Neu im Framework?</strong>
            <span>Beginne mit der Theorie und dem Grundmodell von Bedeutung als semantischem Raum.</span>
          </a>

          <a class="start-card" href="/de/ki-alignment/">
            <strong>Interessierst du dich für KI?</strong>
            <span>Gehe zu KI-Alignment und zur architektonischen Behauptung über innere semantische Pfade.</span>
          </a>

          <a class="start-card" href="/de/kompass/">
            <strong>Willst du den größeren Horizont?</strong>
            <span>Lies den Kompass über Richtung, Urimpuls, Bewusstsein und Emergenz.</span>
          </a>

          <a class="start-card" href="/de/blog/">
            <strong>Willst du die ausführliche Diagnose?</strong>
            <span>Lies Diagnose & Warnung und die Kritik heutiger KI-Architektur.</span>
          </a>

          <a class="start-card" href="/de/buch/">
            <strong>Willst du die menschliche Achse?</strong>
            <span>Gehe zum Buch der Bedeutung und zur größeren existenziellen Entfaltung.</span>
          </a>

          <a class="start-card" href="/de/downloads/">
            <strong>Willst du direkt prüfen?</strong>
            <span>Lade die Dokumente herunter und untersuche das Material im größeren Zusammenhang.</span>
          </a>
        </div>
      </div>
    </div>
  </section>

</div>
