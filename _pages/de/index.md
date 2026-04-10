---
layout: default
title: Semantic Gravitation
permalink: /de/
lang: de
description: "Semantic Gravitation – eine Theorie der Bedeutung als navigierbarer Raum und eine neue Grundlage für KI-Alignment."
translation_url_en: /en/
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
      <p class="home-lead home-lead-plain">Eine Theorie der Bedeutung als navigierbarer Raum — und eine neue Grundlage für KI-Alignment.</p>
    </div>
  </section>

  <section class="section-shell section-shell-tight">
    <div class="hero-research">
      <div class="hero-problem">
        <p>
          KI ist nicht mehr nur ein Werkzeug für Antworten.
          Sie wird Teil der kognitiven Umwelt selbst:
          Teil des Raums, in dem Menschen denken, zweifeln, Probleme rahmen, Wahrheit beurteilen und Orientierung finden.
        </p>
        <p>
          Damit wird semantische Architektur zu einer der zentralen Infrastrukturfragen dieses Jahrhunderts.
          <strong>Welche Art von Bedeutungsraum baut KI um uns herum?</strong>
        </p>
      </div>

      <div class="hero-proof">
        <div class="hero-proof-item"><strong>Bedeutung ist strukturell abbildbar.</strong> Sie ist nicht nur Inhalt, sondern Konfiguration in einem semantischen Zustandsraum.</div>
        <div class="hero-proof-item"><strong>Semantische Zustände sind diagnostisch lesbar.</strong> Sie lassen sich in Spannungen, Trajektorien und Tragfähigkeit beschreiben.</div>
        <div class="hero-proof-item"><strong>Alignment muss innere Pfade betreffen.</strong> Es reicht nicht, Ausgaben erst im Nachhinein zu beurteilen.</div>
      </div>

      <div class="home-cta-row">
        <a class="button" href="/de/theorie/">Zur Theorie</a>
        <a class="button" href="/de/ki-alignment/">KI-Alignment</a>
        <a class="button" href="/de/downloads/">Downloads</a>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="impact-block">
      <p class="display-kicker">Das Problem</p>
      <p class="impact-line">
        Heutige KI beruhigt oft dort,
        wo sie klären müsste.
      </p>
      <p class="impact-sub">
        Edge Alignment versteht Alignment als Navigation durch semantischen Raum —
        nicht nur als Kontrolle von Outputs.
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
      <p class="display-kicker">Was hier neu ist</p>
      <h2 class="section-heading-display">Ein Forschungsprogramm für semantischen Raum</h2>

      <div class="concept-grid">
        <div class="concept-card">
          <p class="concept-card-title">Zustandsraum</p>
          <p class="concept-card-text">Bedeutung ist nicht nur Inhalt, sondern ein strukturierter semantischer Raum aus Positionen, Spannungen und Übergängen.</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">Minimale Grammatik</p>
          <p class="concept-card-text">Kern, Projektion, Relation als kleinste tragfähige semantische Grammatik.</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">Tragfähigkeitsachsen</p>
          <p class="concept-card-text">Kohärenz (Klarheit), Bindung (Würde) und Handlungsfähigkeit (Freiheit) als operative Dimensionen semantischer Zustände.</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">KI-Konsequenz</p>
          <p class="concept-card-text">Alignment verschiebt sich von Antwortkontrolle zu Navigation durch semantischen Raum.</p>
        </div>
      </div>

      <div class="body-copy">
        <p>
          Diese Arbeit beginnt mit einer einfachen, aber weitreichenden Behauptung:
          <strong>Bedeutung ist nicht nur etwas Gesagtes, sondern ein Raum, der strukturiert, kartiert, diagnostiziert und navigiert werden kann.</strong>
        </p>
        <p>
          Edge Alignment ist die KI-architektonische Konsequenz dieser Behauptung.
          Es fragt nicht nur, ob ein System sicher wirkende Outputs erzeugt,
          sondern ob seine inneren Übergänge tragfähig,
          reparierbar
          und an Kohärenz, Bindung und Handlungsfähigkeit ausgerichtet bleiben —
          oder, in öffentlicherer Sprache,
          an Klarheit, Würde und Freiheit.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card">
      <p class="display-kicker">Minimale semantische Grammatik</p>
      <h2 class="section-heading-display">Kern. Projektion. Relation.</h2>

      <div class="section-opening">
        <p>
          Eine der Kernbehauptungen dieses Rahmens lautet, dass beschreibbare Bedeutung immer schon eine minimale Struktur trägt.
        </p>
      </div>

      <p class="display-statement wide">
        Alles, was wir überhaupt beschreiben können,
        läuft implizit durch
        <strong>Kern, Projektion und Relation.</strong>
      </p>

      <div class="concept-grid kpr-grid">
        <div class="concept-card">
          <p class="concept-card-title">Kern</p>
          <p class="concept-card-text">worum es eigentlich geht</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">Projektion</p>
          <p class="concept-card-text">wie etwas sichtbar wird</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">Relation</p>
          <p class="concept-card-text">worin etwas steht und womit es verbunden ist</p>
        </div>
      </div>

      <div class="body-copy">
        <p>
          Das ist hier nicht als lockere Metapher gemeint,
          sondern als Beginn einer formalen semantischen Architektur:
          einer Weise, Zustände, Übergänge, Spannungen und Attraktoren in einem Raum der Bedeutung zu beschreiben.
        </p>
      </div>

      <div class="link-list">
        <a href="/de/theorie/">Tiefer in die Theorie →</a>
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
          Wir haben Systeme gebaut, die Aufmerksamkeit, Rahmung und Denken zunehmend mitformen.
          Was noch fehlt, sind öffentliche semantische Sicherheitsstandards.
        </p>

        <p>
          Nicht nur Systeme, die offensichtlich schlechte Outputs vermeiden,
          sondern Systeme, die <strong>Kohärenz, Bindung und Handlungsfähigkeit</strong>
          im Raum des Denkens selbst bewahren —
          oder, in öffentlicher Sprache,
          <strong>Klarheit, Würde und Freiheit.</strong>
        </p>

        <p>
          Genau deshalb reicht die übliche Sicherheitslogik nicht tief genug.
          Die eigentliche Frage ist nicht nur, ob KI auf offensichtliche Weise gefährlich werden kann,
          sondern ob sie den Raum stiller verengt,
          in dem Menschen sich selbst verstehen,
          Wahrheit beurteilen
          und Orientierung bilden.
        </p>

        <p class="display-statement medium">
          Wir haben das digitale Auto gebaut.
          Der semantische Sicherheitsgurt fehlt noch.
        </p>

        <div class="concept-grid axis-grid">
          <div class="axis-card">
            <h3>Kohärenz (Klarheit)</h3>
            <p>Bleibt der Raum lesbar, differenzierbar und korrigierbar?</p>
          </div>

          <div class="axis-card">
            <h3>Bindung (Würde)</h3>
            <p>Bleibt Beziehung tragfähig, ohne den Menschen herabzusetzen?</p>
          </div>

          <div class="axis-card">
            <h3>Handlungsfähigkeit (Freiheit)</h3>
            <p>Bleiben wirklicher Ausdruck, Korrektur und Bewegung offen?</p>
          </div>
        </div>

        <p class="micro-punch">
          Das sind nicht nur Werte.
          Das sind Tragfähigkeitsachsen.
        </p>
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
          Das ist nicht nur ein Visionstext.
          Hinter der Arbeit stehen bereits prüfbare Materialien.
        </p>

        <div class="proof-grid">
          <div class="proof-card">
            <h3>Theorie-Seite</h3>
            <p>Der begriffliche Einstieg: KPR, semantischer Zustandsraum, Attraktoren, Dekohärenz und tragfähige Übergänge.</p>
          </div>

          <div class="proof-card">
            <h3>Technical Sources</h3>
            <p>Die Quellenebene: die sechs formalen Paper, das separate Alignment-Paper und geschützte Anwendungsrichtungen.</p>
          </div>

          <div class="proof-card">
            <h3>Downloads</h3>
            <p>Gebündelte Prüfkörper für vertieftes Lesen und KI-gestützte Analyse in größerem Zusammenhang.</p>
          </div>
        </div>

        <p class="micro-punch">
          Die Arbeit lässt sich lesen,
          prüfen
          und unabhängig hinterfragen.
        </p>

        <div class="link-list">
          <a href="/de/theorie/">Zur Theorie →</a>
          <a href="/de/papers/">Zu den Technical Sources →</a>
          <a href="/de/downloads/">Zu den Downloads →</a>
        </div>
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
          Es ist ein System, das semantische Räume selbst rekonstruieren,
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
        <strong>Mehr Lesbarkeit.</strong>
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

          <a class="start-card" href="/de/blog/">
            <strong>Willst du die ausführliche Diagnose?</strong>
            <span>Lies Manifest, Diagnose und Kritik heutiger KI-Architektur.</span>
          </a>

          <a class="start-card" href="/de/downloads/">
            <strong>Willst du die Arbeit direkt prüfen?</strong>
            <span>Lade die Dokumente herunter und untersuche das Material im größeren Zusammenhang.</span>
          </a>
        </div>
      </div>
    </div>
  </section>

</div>
