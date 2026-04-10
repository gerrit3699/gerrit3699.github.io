---
layout: default
title: "Kontakt & Unterstützung"
permalink: /de/kontakt/
lang: de
description: "Kontakt zu Gerrit Klawitter, Semantische Gravitation, Unterstützung, Zusammenarbeit und PayPal."
translation_url_en: /en/contact/
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
      <p class="contact-kicker">Kontakt & Unterstützung</p>
      <h1 class="contact-display">Nimm Kontakt auf.</h1>
      <p class="contact-sublead">
        Für Kontakt, Resonanz, Zusammenarbeit, Unterstützung
        und ernsthafte Angebote, dabei zu helfen,
        aus der Semantischen Gravitation etwas strukturell Reales zu machen.
      </p>

      <div class="claim-grid">
        <a class="claim-card" href="#kontakt">
          <h3>Kontakt</h3>
          <p>Schreib, wenn dich die Arbeit erreicht hat, wenn du eine ernsthafte Frage hast oder Verbindung aufnehmen möchtest.</p>
        </a>
        <a class="claim-card" href="#unterstuetzung">
          <h3>Unterstützung</h3>
          <p>Finanzielle Unterstützung macht in dieser Phase einen sehr realen Unterschied.</p>
        </a>
        <a class="claim-card" href="#mitbauen">
          <h3>Mitbauen</h3>
          <p>Kontakte, Reichweite, Struktur, Herz, Strategie, Medien und technische Zusammenarbeit sind alle relevant.</p>
        </a>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="contact-block">
      <h2 class="section-heading-display">Aktuelle Situation</h2>

      <div class="body-copy">
        <p>
          Die Semantische Gravitation wird noch unter sehr realen Bedingungen aufgebaut.
          Zurzeit arbeite ich weitgehend allein daran:
          an Website, Papern, Architektur, Texten, öffentlicher Rahmung, Downloads, Positionierung
          und an den nächsten strukturellen Schritten.
        </p>

        <p>
          Freunde helfen mir hier und da bei philosophischen Fragen,
          bei Formulierungen
          und mit Feedback.
          Das Projekt selbst trage ich im Kern aber noch allein.
        </p>

        <p>
          Gleichzeitig halte ich mich derzeit noch mit Jobs über Wasser.
          Hinter diesem Projekt steht noch kein echtes Team,
          keine stabile Finanzierung
          und keine größere institutionelle Struktur.
          Vieles ist über viele Monate hinweg durch anhaltende Arbeit entstanden,
          oft mit acht bis zehn Stunden täglich,
          wann immer es möglich war.
        </p>
      </div>

      <p class="display-statement wide">
        Die Arbeit ist real.
        Die Struktur darum muss noch gebaut werden.
      </p>

      <div class="status-box">
        <p class="status-label">Was das praktisch bedeutet</p>
        <p>
          Unterstützung, Kontakte, Finanzierung, Sichtbarkeit und ernsthafte Zusammenarbeit helfen im Moment nicht abstrakt.
          Sie helfen sehr konkret.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell" id="kontakt">
    <div class="contact-block">
      <h2 class="section-heading-display">Kontakt</h2>

      <div class="body-copy">
        <p>
          Wenn dich die Arbeit auf <strong>semanticgravitation.org</strong> anspricht,
          wenn du Resonanz spürst,
          ernsthaftes Feedback geben möchtest,
          Kontakte einbringen willst,
          das Projekt unterstützen möchtest
          oder einen Weg siehst, wie du helfen kannst,
          kannst du mich hier erreichen.
        </p>
      </div>

      <div class="contact-links">
        <a class="contact-link" href="mailto:contact@semanticgravitation.org">
          <strong>E-Mail:</strong> contact@semanticgravitation.org
        </a>

        <a class="contact-link" href="https://instagram.com/semanticgravitation" target="_blank" rel="noopener">
          <strong>Instagram:</strong> @semanticgravitation
        </a>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell" id="mitbauen">
    <div class="contact-block">
      <h2 class="section-heading-display">Wie du helfen kannst</h2>

      <div class="support-grid">
        <div class="support-card">
          <h3>Kontakte & Reichweite</h3>
          <p>Bring die Arbeit zu den richtigen Menschen, Netzwerken, Institutionen, Aufbauenden oder öffentlichen Denkern.</p>
        </div>
        <div class="support-card">
          <h3>Aufbau & Struktur</h3>
          <p>Hilf bei Organisation, Website, Medien, technischem Ausbau, Design, öffentlicher Kommunikation oder Operations.</p>
        </div>
        <div class="support-card">
          <h3>Finanzierung & Unterstützung</h3>
          <p>Hilf dabei, den finanziellen Raum zu schaffen, in dem daraus etwas kontinuierlicher, öffentlicher und baubar werden kann.</p>
        </div>
      </div>

      <div class="body-copy">
        <p>
          Du brauchst keine vorab festgelegte Rolle, um zu schreiben.
          Wenn du dich von dieser Arbeit ernsthaft angesprochen fühlst,
          kannst du auch einfach sagen, was du einbringen kannst.
        </p>

        <p>
          Ich möchte nicht alles sofort in starre Boxen pressen.
          Mit der Zeit soll ein Feld entstehen,
          in dem klarere Rollen, Verantwortlichkeiten und Formen der Zusammenarbeit wachsen können.
          Im Moment ist ein Teil der Aufgabe aber schlicht,
          dass der richtige Kontakt überhaupt sichtbar wird.
        </p>
      </div>

      <p class="display-statement medium">
        Wenn du dich gerufen fühlst,
        schreib.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell" id="unterstuetzung">
    <div class="contact-block">
      <h2 class="section-heading-display">Unterstützung</h2>

      <div class="body-copy">
        <p>
          Wenn du meine Arbeit direkt unterstützen möchtest,
          kannst du das hier tun.
        </p>

        <p>
          Deine Unterstützung hilft dabei,
          Zeit, Energie und Infrastruktur für dieses Projekt tragfähiger zu machen:
          für Forschung, Schreiben, Veröffentlichung, Website, öffentliche Kommunikation,
          die Weiterentwicklung der Architektur
          und den langfristigen Aufbau der Semantischen Gravitation.
        </p>

        <p>
          Gerade in dieser Phase macht Unterstützung einen realen Unterschied.
          Sie senkt Druck,
          schafft Raum
          und macht es realistischer,
          diese Arbeit nicht nur neben allem anderen,
          sondern mit mehr Kontinuität, Tiefe und Reichweite in die Welt zu bringen.
        </p>

        <p>
          Ich werde diese Arbeit so oder so weiterführen.
          Aber wenn dich dieses Projekt berührt,
          wenn du es für wichtig hältst
          oder dabei helfen willst, dass daraus etwas Tragfähiges wächst,
          dann hilft dein Beitrag im Moment sehr konkret.
        </p>
      </div>

      <a class="support-link" href="https://paypal.me/semanticgravitation" target="_blank" rel="noopener">
        Meine Arbeit unterstützen
      </a>

      <div class="body-copy">
        <p>
          <a href="https://paypal.me/semanticgravitation" target="_blank" rel="noopener">paypal.me/semanticgravitation</a>
        </p>

        <p>
          Im Moment ist Unterstützung am besten als freiwilliger Beitrag zu verstehen,
          der diese Arbeit ermöglicht und weiterentwickelt.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="contact-block">
      <h2 class="section-heading-display">Bevor du schreibst</h2>

      <div class="body-copy">
        <p>
          Ich schätze ernsthafte Nachrichten.
          Was ich im Moment aber weder leisten kann noch leisten möchte,
          ist, in einzelnen Gesprächen immer wieder ganz von vorn zu erklären,
          was die Semantische Gravitation ist,
          warum sie funktionieren könnte
          oder wie sich jeder einzelne Baustein im Detail herleitet.
        </p>

        <p>
          Wenn du wirklich verstehen willst, worum es hier geht,
          nutze bitte zuerst die Materialien auf der Seite:
          besonders die Theorie-Seite,
          die Technischen Quellen,
          die Downloads
          und das Alignment-Material.
        </p>

        <p>
          Mein Vorschlag ist:
          Nimm deine wirkliche Frage,
          lade die Dokumente in eine KI deiner Wahl,
          arbeite dich selbst in das Material hinein
          und prüfe den Punkt,
          der dich wirklich interessiert, irritiert oder ruft.
        </p>

        <p>
          Glaube nicht zu schnell.
          Lehne nicht zu schnell ab.
          Aber frage präzise,
          prüfe sorgfältig
          und nimm deinen eigenen Kurzschluss als Ausgangspunkt für die nächste bessere Frage.
        </p>
      </div>

      <div class="status-box">
        <p class="status-label">Eine gute Nachricht hilft</p>
        <p>
          Was hat dich erreicht?
          Was ist dir wichtig?
          Was kannst du beitragen, fragen, verbinden oder mit in Bewegung setzen?
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="closing-block">
      <h2 class="section-heading-display">Hinweis</h2>

      <div class="body-copy">
        <p>
          Ich lese Nachrichten so gut ich kann.
          Gerade in intensiveren Phasen kann eine Antwort etwas Zeit brauchen.
        </p>

        <p>
          Klare, konkrete und ehrliche Nachrichten helfen am meisten.
          Ernsthafte Resonanz ist willkommen.
          Ernsthafte Hilfe ist willkommen.
          Ernsthafte Unterstützung ist willkommen.
        </p>
      </div>
    </div>
  </section>

</div>
