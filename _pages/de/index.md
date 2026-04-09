---
layout: default
title: Semantic Gravitation
permalink: /de/
lang: de
description: "Semantic Gravitation – eine Theorie von Bedeutung als navigierbarem Raum und eine neue Grundlage für KI-Alignment."
---

<style>
  .home-journey {
    --sg-text: rgba(255,255,255,0.97);
    --sg-soft: rgba(255,255,255,0.78);
    --sg-dim: rgba(255,255,255,0.64);
    --sg-line: rgba(255,255,255,0.10);
    --sg-line-strong: rgba(255,255,255,0.16);
    --sg-panel: rgba(255,255,255,0.035);
    --sg-panel-strong: rgba(255,255,255,0.05);
    --sg-max: 1120px;
    --sg-copy: 860px;
    --sg-wide: 980px;
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
    gap: 1.6rem;
  }

  .home-journey .hero-problem {
    max-width: 46rem;
    font-size: clamp(1.28rem, 2.5vw, 1.8rem);
    line-height: 1.5;
    letter-spacing: -0.025em;
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
    margin-top: 0.35rem;
  }

  .home-journey .hero-proof-item {
    font-size: clamp(1.02rem, 1.8vw, 1.16rem);
    line-height: 1.5;
    color: var(--sg-text);
  }

  .home-journey .hero-proof-item strong {
    font-weight: 760;
  }

  .home-journey .home-cta-row {
    display: flex;
    flex-wrap: wrap;
    gap: 0.9rem;
    margin-top: 0.8rem;
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
    max-width: 10.5ch;
    font-size: clamp(2.55rem, 6.6vw, 5.6rem);
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
    line-height: 1.6;
    color: var(--sg-text);
  }

  .home-journey .impact-question strong {
    display: inline-block;
    margin-top: 0.15rem;
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
    max-width: 52rem;
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
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1rem;
    margin: 1.8rem 0 2rem;
  }

  .home-journey .concept-card,
  .home-journey .axis-card {
    padding: 1.15rem 1.05rem 1.05rem;
    border-radius: 22px;
    background: linear-gradient(180deg, rgba(255,255,255,0.05) 0%, rgba(255,255,255,0.028) 100%);
    border: 1px solid var(--sg-line);
    box-shadow:
      0 18px 48px rgba(0,0,0,0.18),
      inset 0 1px 0 rgba(255,255,255,0.03);
  }

  .home-journey .concept-card-title,
  .home-journey .axis-card h3 {
    margin: 0 0 0.45rem;
    font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
    font-size: 1.5rem;
    line-height: 1.02;
    letter-spacing: -0.04em;
    font-weight: 760;
  }

  .home-journey .concept-card-text,
  .home-journey .axis-card p {
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
    .home-journey .concept-grid,
    .home-journey .proof-grid,
    .home-journey .start-grid {
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
      font-size: 1rem;
      line-height: 1.48;
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
      max-width: 8.8ch;
      font-size: 3.25rem;
      line-height: 0.93;
    }

    .home-journey .impact-sub {
      font-size: 1.15rem;
      max-width: 19ch;
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
    .home-journey .start-card {
      border-radius: 18px;
      padding: 1rem 0.95rem 0.95rem;
    }
  }
</style>

<div class="home-journey">

  <section class="hero home-hero section-fog">
    <div class="hero-inner">
      <h1 class="display-wordmark">Semantic<br>Gravitation</h1>
      <p class="home-lead">Eine Theorie von Bedeutung als navigierbarem Raum — und eine neue Grundlage für KI-Alignment.</p>
    </div>
  </section>

  <section class="section-shell section-shell-tight">
    <div class="hero-research">
      <div class="hero-problem">
        <p>
          KI ist nicht mehr nur ein Werkzeug für Antworten.
          Sie wird Teil des Raums, in dem Menschen denken, zweifeln, Probleme rahmen und Orientierung bilden.
        </p>
        <p>
          Darum gehört zu den zentralen Fragen dieses Jahrhunderts:
          <strong>Welche Art von semantischem Raum baut KI um uns herum?</strong>
        </p>
      </div>

      <div class="hero-proof">
        <div class="hero-proof-item"><strong>Bedeutung ist nicht nur Inhalt.</strong> Sie ist Struktur. Sie ist ein Raum.</div>
        <div class="hero-proof-item"><strong>Semantische Zustände lassen sich kartieren und bewerten.</strong> Sie sind nicht nur Stimmung oder Metapher.</div>
        <div class="hero-proof-item"><strong>Alignment muss innere Wege betreffen, nicht nur Outputs.</strong> Genau dort beginnt Edge Alignment.</div>
      </div>

      <div class="home-cta-row">
        <a class="button" href="/de/theorie/">Zur Theorie</a>
        <a class="button" href="/de/ki-alignment/">Zu Alignment</a>
        <a class="button" href="/de/downloads/">Papers herunterladen</a>
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
        Die entscheidende Frage ist nicht nur, ob eine Antwort akzeptabel wirkt,
        sondern <strong>durch welchen Bedeutungsraum ein System gegangen ist, um dort anzukommen.</strong>
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="free-text-block">
      <p class="display-kicker">Was hier neu ist</p>
      <h2 class="section-heading-display">Ein Forschungsprogramm für semantischen Raum</h2>

      <div class="concept-grid">
        <div class="concept-card">
          <p class="concept-card-title">Bedeutung als Raum</p>
          <p class="concept-card-text">Nicht nur Inhalt, sondern Struktur, Topologie, Übergang und Richtung.</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">Eine Minimalgrammatik</p>
          <p class="concept-card-text">Kern, Projektion, Relation als kleinste tragfähige semantische Grammatik.</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">Ein neues KI-Modell</p>
          <p class="concept-card-text">Vom Antwortautomaten hin zu Systemen, die semantischen Raum lesen und navigieren.</p>
        </div>
      </div>

      <div class="body-copy">
        <p>
          Diese Arbeit beginnt mit einer einfachen, aber weitreichenden Behauptung:
          <strong>Bedeutung ist nicht nur etwas Gesagtes, sondern ein Raum, der strukturierbar, kartierbar und navigierbar ist.</strong>
        </p>
        <p>
          Edge Alignment ist die KI-Anwendung dieser Behauptung.
          Es fragt nicht nur, ob ein System sichere oder gefällige Outputs erzeugt,
          sondern ob seine inneren Übergänge tragfähig, reparierbar
          und an Klarheit, Würde und Freiheit ausgerichtet bleiben.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="free-text-block">
      <p class="display-kicker">Minimale semantische Grammatik</p>
      <h2 class="section-heading-display">Kern. Projektion. Relation.</h2>

      <div class="section-opening">
        <p>
          Eine der Kernthesen dieses Rahmens ist:
          Beschreibbare Bedeutung trägt immer schon eine minimale Struktur.
        </p>
      </div>

      <p class="display-statement wide">
        Alles, was wir überhaupt beschreiben können,
        läuft implizit über
        <strong>Kern, Projektion und Relation.</strong>
      </p>

      <div class="concept-grid">
        <div class="concept-card">
          <p class="concept-card-title">Kern</p>
          <p class="concept-card-text">worum es eigentlich geht</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">Projektion</p>
          <p class="concept-card-text">wie es sichtbar wird</p>
        </div>
        <div class="concept-card">
          <p class="concept-card-title">Relation</p>
          <p class="concept-card-text">worin es in Beziehung steht</p>
        </div>
      </div>

      <div class="body-copy">
        <p>
          Das ist hier nicht als lose Metapher gemeint,
          sondern als Anfang einer formalen semantischen Architektur:
          einer Weise, Zustände, Übergänge, Spannungen und Attraktoren
          in einem Bedeutungsraum zu beschreiben.
        </p>
      </div>

      <div class="link-list">
        <a href="/de/theorie/">Tiefe Theorie lesen →</a>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="section-card section-bubbles-strong">
      <div class="section-head">
        <h2>Warum das gerade jetzt wichtig ist</h2>
      </div>

      <div class="section-body body-copy">
        <p class="section-intro">
          Wir haben Systeme gebaut, die Aufmerksamkeit, Rahmung und Denken immer stärker mitprägen.
          Was bisher fehlt, sind semantische Sicherheitsstandards.
        </p>

        <p>
          Nicht nur Systeme, die schlechte oder riskante Outputs vermeiden,
          sondern Systeme, die <strong>Klarheit, Würde und Freiheit</strong>
          im Denkraum selbst erhalten.
        </p>

        <p>
          Genau deshalb liegt das Problem tiefer, als gewöhnliche Safety-Sprache nahelegt.
          Die eigentliche Frage ist nicht nur, ob KI in offensichtlicher Weise gefährlich werden kann,
          sondern ob sie leise den Raum verengt,
          in dem Menschen sich selbst verstehen, Wahrheit prüfen und Orientierung bilden.
        </p>

        <p class="display-statement medium">
          Wir haben das digitale Auto gebaut.
          Der semantische Sicherheitsgurt fehlt noch.
        </p>

        <div class="section-grid grid-3">
          <div class="axis-card">
            <h3>Klarheit</h3>
            <p>Kann der Raum noch klar gesehen und geprüft werden?</p>
          </div>

          <div class="axis-card">
            <h3>Würde</h3>
            <p>Erhält das System Beziehung, ohne den Menschen zu verkleinern?</p>
          </div>

          <div class="axis-card">
            <h3>Freiheit</h3>
            <p>Bleiben Ausdruck, Korrektur und reale Bewegung offen?</p>
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
    <div class="section-card section-field">
      <div class="section-head">
        <h2>Was schon geprüft werden kann</h2>
      </div>

      <div class="section-body body-copy">
        <p class="section-intro">
          Das ist nicht nur eine Vision.
          Dahinter liegen bereits prüfbare Materialien.
        </p>

        <div class="proof-grid">
          <div class="proof-card">
            <h3>Collected Papers I–VI</h3>
            <p>Das theoretische Rückgrat von Semantic Gravitation als zusammenhängende Forschungslinie.</p>
          </div>

          <div class="proof-card">
            <h3>Edge Alignment Paper</h3>
            <p>Der KI-Architekturanspruch in verdichteter Form: Navigation, Drift und semantische Safety-Architekturen.</p>
          </div>

          <div class="proof-card">
            <h3>Theorie-Seite</h3>
            <p>Begriffe wie KPR, Setzungen, Attraktoren, Dekohärenz und tragfähige Übergänge.</p>
          </div>
        </div>

        <p class="micro-punch">
          Die Arbeit kann gelesen,
          geprüft
          und unabhängig gespiegelt werden.
        </p>

        <div class="link-list">
          <a href="/de/downloads/">Zu den Downloads →</a>
          <a href="/de/papers/">Zu Papers & Patenten →</a>
        </div>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="free-text-block">
      <p class="display-kicker">Systemrichtung</p>
      <h2 class="section-heading-display">Vom Antwortautomaten zum semantischen Raumscanner</h2>

      <div class="body-copy">
        <p>
          Das langfristige Systembild hinter dieser Arbeit ist nicht bloß ein besserer Chatbot.
          Gemeint ist ein System, das semantischen Raum selbst rekonstruieren,
          lesen und navigieren kann.
        </p>

        <p>
          Das heißt:
          weniger Nebel,
          weniger versteckte Lenkung,
          weniger Pseudoklarheit aus Ausblendung —
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
    <div class="section-card section-fog">
      <div class="section-head">
        <h2>Hier anfangen</h2>
      </div>

      <div class="section-body">
        <div class="start-grid">
          <a class="start-card" href="/de/theorie/">
            <strong>Neu im Rahmen?</strong>
            <span>Starte mit der Theorie und dem Grundmodell von Bedeutung als semantischem Raum.</span>
          </a>

          <a class="start-card" href="/de/ki-alignment/">
            <strong>Interesse an KI?</strong>
            <span>Gehe zu Alignment und zum Architekturanspruch über innere semantische Wege.</span>
          </a>

          <a class="start-card" href="/de/blog/">
            <strong>Willst du die Langdiagnose?</strong>
            <span>Lies das Manifest und die Kritik an heutiger KI-Architektur.</span>
          </a>

          <a class="start-card" href="/de/downloads/">
            <strong>Willst du die Arbeit direkt prüfen?</strong>
            <span>Lade die Papers herunter und arbeite mit dem Material im vollen Kontext.</span>
          </a>
        </div>
      </div>
    </div>
  </section>

</div>
