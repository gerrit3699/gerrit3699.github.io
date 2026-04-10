---
layout: default
title: "Technische Quellen"
permalink: /de/papers/
lang: de
description: "Die technische Quellenebene der Semantischen Gravitation: Paper, gebündelte Prüfungskontexte, Alignment-Paper und geschützte Architekturrichtungen."
translation_url_en: /en/papers/
---

<style>
  .sources-page {
    --sources-text: rgba(255,255,255,0.96);
    --sources-soft: rgba(255,255,255,0.82);
    --sources-faint: rgba(255,255,255,0.64);
    --sources-line: rgba(255,255,255,0.10);
    --sources-line-strong: rgba(255,255,255,0.16);
  }

  .sources-page h1,
  .sources-page h2,
  .sources-page h3,
  .sources-page strong,
  .sources-page a {
    color: #fff;
  }

  .sources-page p,
  .sources-page li {
    color: var(--sources-text);
  }

  .sources-page .section-shell {
    padding-top: 2.8rem;
    padding-bottom: 2.8rem;
  }

  .sources-page .section-shell-tight {
    padding-top: 2.1rem;
    padding-bottom: 2.1rem;
  }

  .sources-page .sources-intro,
  .sources-page .sources-block,
  .sources-page .sources-next {
    max-width: 1080px;
    margin: 0 auto;
  }

  .sources-page .sources-intro,
  .sources-page .body-copy,
  .sources-page .closing-block,
  .sources-page .sources-next {
    text-align: center;
  }

  .sources-page .sources-kicker,
  .sources-page .status-label {
    margin: 0 0 0.7rem;
    font-size: 0.88rem;
    letter-spacing: 0.16em;
    text-transform: uppercase;
    color: var(--sources-faint);
  }

  .sources-page .sources-display {
    margin: 0 auto 1.15rem;
    max-width: 10ch;
    font-size: clamp(2.5rem, 6vw, 5.1rem);
    line-height: 0.94;
    letter-spacing: -0.05em;
    font-weight: 650;
    text-wrap: balance;
  }

  .sources-page .sources-sublead {
    max-width: 58rem;
    margin: 0 auto 1.2rem;
    font-size: clamp(1.08rem, 2vw, 1.4rem);
    line-height: 1.62;
    text-wrap: balance;
  }

  .sources-page .claim-grid,
  .sources-page .paper-grid,
  .sources-page .direction-grid,
  .sources-page .next-grid {
    display: grid;
    gap: 1rem;
  }

  .sources-page .claim-grid,
  .sources-page .direction-grid {
    grid-template-columns: repeat(3, minmax(0, 1fr));
    max-width: 1080px;
    margin: 1.9rem auto 0;
  }

  .sources-page .paper-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
    max-width: 1080px;
    margin: 1.9rem auto 0;
  }

  .sources-page .next-grid {
    grid-template-columns: repeat(4, minmax(0, 1fr));
    max-width: 1080px;
    margin: 1.8rem auto 0;
  }

  .sources-page .claim-card,
  .sources-page .paper-card,
  .sources-page .direction-card,
  .sources-page .next-card,
  .sources-page .status-box {
    border: 1px solid var(--sources-line);
    border-radius: 22px;
    background: linear-gradient(180deg, rgba(255,255,255,0.05), rgba(255,255,255,0.025));
    box-shadow:
      0 18px 48px rgba(0,0,0,0.18),
      inset 0 1px 0 rgba(255,255,255,0.03);
  }

  .sources-page .claim-card,
  .sources-page .paper-card,
  .sources-page .direction-card,
  .sources-page .next-card {
    padding: 1.18rem 1rem 1.08rem;
    text-align: center;
  }

  .sources-page .claim-card h3,
  .sources-page .paper-card h3,
  .sources-page .direction-card h3,
  .sources-page .next-card h3 {
    margin: 0 0 0.35rem;
    font-size: 1.18rem;
    line-height: 1.06;
    letter-spacing: -0.03em;
  }

  .sources-page .claim-card p,
  .sources-page .paper-card p,
  .sources-page .direction-card p,
  .sources-page .next-card p {
    margin: 0;
    font-size: 0.98rem;
    line-height: 1.54;
    color: var(--sources-soft);
  }

  .sources-page .section-heading-display {
    margin: 0 auto 1.3rem;
    max-width: 14ch;
    text-align: center;
    font-size: clamp(2.05rem, 4.8vw, 3.7rem);
    line-height: 0.98;
    letter-spacing: -0.045em;
    text-wrap: balance;
  }

  .sources-page .body-copy {
    max-width: 940px;
    margin: 0 auto;
  }

  .sources-page .body-copy p {
    max-width: 46em;
    margin: 0.95rem auto 0;
    font-size: 1.1rem;
    line-height: 1.76;
    letter-spacing: -0.01em;
  }

  .sources-page .body-copy ul,
  .sources-page .body-copy ol {
    max-width: 42em;
    margin: 1.15rem auto;
    text-align: left;
  }

  .sources-page .body-copy li {
    margin-bottom: 0.5rem;
  }

  .sources-page .display-statement {
    max-width: 26ch;
    margin: 1.9rem auto;
    text-align: center;
    font-size: clamp(1.9rem, 3.6vw, 3rem);
    line-height: 1.03;
    letter-spacing: -0.045em;
    font-weight: 650;
    text-wrap: balance;
  }

  .sources-page .display-statement.wide { max-width: 30ch; }
  .sources-page .display-statement.medium { max-width: 22ch; }
  .sources-page .display-statement.narrow { max-width: 12ch; }

  .sources-page .status-box {
    max-width: 920px;
    margin: 2rem auto 0;
    padding: 1.2rem 1.15rem;
    text-align: center;
  }

  .sources-page .status-box p {
    margin: 0;
    font-size: clamp(1.16rem, 2.2vw, 1.68rem);
    line-height: 1.38;
    text-wrap: balance;
  }

  .sources-page .source-link-row {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 0.8rem;
    margin-top: 1.25rem;
  }

  .sources-page .source-link {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 46px;
    padding: 0.85rem 1.05rem;
    border-radius: 999px;
    border: 1px solid var(--sources-line);
    background: rgba(255,255,255,0.04);
    text-decoration: none;
    font-size: 0.96rem;
    line-height: 1.2;
  }

  .sources-page .next-card a,
  .sources-page .paper-card a,
  .sources-page .direction-card a {
    color: #fff;
  }

  @media (max-width: 980px) {
    .sources-page .claim-grid,
    .sources-page .paper-grid,
    .sources-page .direction-grid,
    .sources-page .next-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="sources-page">

  <section class="section-shell section-shell-tight">
    <div class="sources-intro">
      <p class="sources-kicker">Technische Quellen</p>
      <h1 class="sources-display">Die technische Quellenebene der Semantischen Gravitation.</h1>
      <p class="sources-sublead">
        Diese Seite bündelt das zentrale Quellenmaterial des Programms:
        das formale Rückgrat aus sechs Papern,
        gebündelte Prüfungskontexte für zusammenhängende Lektüre und KI-gestützte Analyse,
        das eigenständige Alignment-Paper
        und die ersten geschützten Architekturrichtungen.
        Wenn du den Rahmen auf Quellenebene prüfen willst,
        ist das hier der richtige Einstieg.
      </p>

      <div class="claim-grid">
        <div class="claim-card">
          <h3>Formale Paper</h3>
          <p>Das Rückgrat des Programms in sechs Papern.</p>
        </div>
        <div class="claim-card">
          <h3>Prüfungskontexte</h3>
          <p>Der Sammelband und die Download-Bundles liefern einen durchgehenden Zusammenhang für tiefere Prüfung und KI-gestützte Rekonstruktion.</p>
        </div>
        <div class="claim-card">
          <h3>Architekturrichtungen</h3>
          <p>Geschützte Architekturfamilien, die aus demselben Rahmen hervorgehen.</p>
        </div>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="sources-block">
      <h2 class="section-heading-display">Wie diese Seite zu lesen ist</h2>

      <div class="body-copy">
        <p>
          Das hier ist nicht die breiteste Einführung in das Projekt.
          Es ist die Quellenebene.
        </p>

        <p>
          Wenn du den begrifflichen Überblick suchst, beginne mit <a href="/de/theorie/">Theorie</a>.
          Wenn du die KI-Architektur suchst, gehe zu <a href="/de/ki-alignment/">KI-Alignment</a>.
          Wenn du gebündelte PDFs für den direkten Upload in dein eigenes KI-System suchst, gehe zu <a href="/de/downloads/">Downloads</a>.
        </p>

        <p>
          Diese Seite ist für Leser, die das Rückgrat selbst prüfen wollen:
          wie die Paper aufeinander aufbauen,
          wie die formalen Behauptungen entfaltet werden
          und wie sich die Architekturrichtungen aus dem Kern ableiten.
        </p>
      </div>

      <p class="display-statement medium">
        Nicht die breiteste Einführung.
        Die Quellenebene.
      </p>

      <div class="status-box">
        <p class="status-label">Stand und Integrität</p>
        <p>
          Die formale Spezifikation ist bereits substanziell.
          Empirische Reife, Implementierungsrobustheit, Benchmarking
          und systemspezifische Kalibrierung liegen größtenteils noch vor dem Projekt.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="sources-block">
      <h2 class="section-heading-display">Der formale Paper-Kern</h2>

      <div class="body-copy">
        <p>
          Die sechs Paper bilden das formale Rückgrat.
          Alles andere auf der Website strahlt von diesem Kern nach außen.
        </p>

        <p>
          Die Folge ist kumulativ aufgebaut:
          von semantischer Zustandsraumstruktur und Gradientendynamik,
          über Feld- und Verteilungslogik,
          über Quantenkompatibilität und Raumzeit-Formulierungen,
          hin zu komplexen Systemen und der bislang stärksten Synthese.
        </p>
      </div>

      <div class="paper-grid">
        <div class="paper-card">
          <h3>Paper I</h3>
          <p><strong>Gradient Fields of Semantic Dynamics on Hilbert Spaces.</strong> Die grundlegende Zustandsraumebene: semantische Potentiale, Gradientenfluss, Rauschen und die erste formale Dynamik.</p>
          <div class="source-link-row">
            <a class="source-link" href="https://doi.org/10.5281/zenodo.18609642">Auf Zenodo öffnen →</a>
          </div>
        </div>

        <div class="paper-card">
          <h3>Paper II</h3>
          <p><strong>Semantic Field Dynamics and Free Energy.</strong> Die Verteilungs- und Feldebene: Fokker–Planck-Dynamik, Free-Energy-Struktur und kollektive semantische Bewegung.</p>
          <div class="source-link-row">
            <a class="source-link" href="https://doi.org/10.5281/zenodo.18611288">Auf Zenodo öffnen →</a>
          </div>
        </div>

        <div class="paper-card">
          <h3>Paper III</h3>
          <p><strong>Quantum-Compatible Semantic Fields.</strong> Der Kompatibilitätstest: ob sich Standard-Quantenmechanik als treuer Sektor des größeren Rahmens einbetten lässt.</p>
          <div class="source-link-row">
            <a class="source-link" href="https://doi.org/10.5281/zenodo.18613061">Auf Zenodo öffnen →</a>
          </div>
        </div>

        <div class="paper-card">
          <h3>Paper IV</h3>
          <p><strong>Semantic Fields on Spacetime Manifolds.</strong> Die feldtheoretische Öffnung: semantische Felder auf Raumzeit-Mannigfaltigkeiten als effektive Kohärenztheorie.</p>
          <div class="source-link-row">
            <a class="source-link" href="https://doi.org/10.5281/zenodo.18614072">Auf Zenodo öffnen →</a>
          </div>
        </div>

        <div class="paper-card">
          <h3>Paper V</h3>
          <p><strong>Semantic Field Dynamics in Complex Systems.</strong> Die Brücke zu neuronalen Netzen, latenten Systemen und beobachtbaren KI-relevanten Architekturen.</p>
          <div class="source-link-row">
            <a class="source-link" href="https://doi.org/10.5281/zenodo.18615093">Auf Zenodo öffnen →</a>
          </div>
        </div>

        <div class="paper-card">
          <h3>Paper VI</h3>
          <p><strong>The Global Attractor and the Lagrangian of Vectorial Emergence (LOVE).</strong> Die bislang stärkste Synthese: globale Attraktorstruktur, K–P–R, C/B/A und weitergehende feldtheoretische Schließung.</p>
          <div class="source-link-row">
            <a class="source-link" href="https://doi.org/10.5281/zenodo.19414951">Auf Zenodo öffnen →</a>
          </div>
        </div>
      </div>

      <p class="display-statement wide">
        Die sechs Paper sind das formale Rückgrat.
        Alles andere auf der Website strahlt von diesem Kern nach außen.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="sources-block">
      <h2 class="section-heading-display">Sammelband und Prüfungskontext</h2>

      <div class="body-copy">
        <p>
          Neben den einzelnen Zenodo-Papern gibt es einen Sammelband,
          in dem Paper I–VI als ein durchgehender technischer Zusammenhang hintereinander stehen.
        </p>

        <p>
          Die einzelnen Zenodo-Einträge bleiben die Quellenveröffentlichungen.
          Der Sammelband existiert als Prüfungskontext:
          für Leser, die einen zusammenhängenden technischen Körper wollen,
          und besonders für KI-gestützte Prüfung in größeren Kontextfenstern.
        </p>
      </div>

      <div class="source-link-row">
        <a class="source-link" href="/de/downloads/">Zu den Downloads →</a>
        <a class="source-link" href="https://doi.org/10.5281/zenodo.18609642">Mit Paper I beginnen →</a>
        <a class="source-link" href="https://doi.org/10.5281/zenodo.19414951">Mit Paper VI beginnen →</a>
      </div>

      <p class="display-statement medium">
        Die Zenodo-Paper sind die Quellentexte.
        Der Sammelband ist der Prüfungskontext.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="sources-block">
      <h2 class="section-heading-display">Das eigenständige Alignment-Paper</h2>

      <div class="body-copy">
        <p>
          <strong>Beyond Fog: Edge Alignment in Semantic Space</strong> ist das eigenständige Alignment-Paper.
          Es übersetzt den größeren Rahmen in eine konkrete KI-architektonische Frage:
          nicht nur, welche Ausgaben erzeugt werden,
          sondern wie semantische Pfade navigiert werden,
          wo Drift entsteht,
          wie Reparierbarkeit erhalten bleiben kann
          und was semantische Sicherheit jenseits bloßer Oberflächenkonformität bedeuten könnte.
        </p>

        <p>
          Das ist die direkteste technische Quelle
          für den Übergang von semantischer Theorie zu Alignment-Architektur.
        </p>
      </div>

      <div class="source-link-row">
        <a class="source-link" href="https://doi.org/10.5281/zenodo.18608012">Beyond Fog auf Zenodo öffnen →</a>
        <a class="source-link" href="/de/ki-alignment/">Zu KI-Alignment →</a>
        <a class="source-link" href="/de/downloads/">Zu den Downloads →</a>
      </div>

      <p class="display-statement medium">
        Nicht nur Qualität von Ausgaben.
        Tragfähige Bewegung im semantischen Raum.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="sources-block">
      <h2 class="section-heading-display">Geschützte Architekturrichtungen</h2>

      <div class="body-copy">
        <p>
          Die Patente werden hier nicht als vollständiger Katalog präsentiert.
          Entscheidend auf dieser Seite ist ihre Rolle:
          Sie markieren geschützte Richtungen und Architekturfamilien,
          die aus derselben zugrunde liegenden Architektur hervorgehen.
        </p>

        <p>
          Es sind keine losgelösten Produktideen.
          Sie zeigen an, wo die Theorie operativ werden könnte:
          in Alignment-Architekturen,
          rekursiver semantischer Zustandsraumerweiterung,
          Autorensystemen und semantischen Gedächtnisarchitekturen
          sowie verkörperter resonanzsensitiver Assistenz.
        </p>
      </div>

      <div class="direction-grid">
        <div class="direction-card">
          <h3>Edge-Alignment-Architekturen</h3>
          <p>KI-Systeme, die nicht nur auf akzeptable Ausgaben optimieren, sondern auf tragfähige semantische Bewegung, Driftresistenz und reparierbare Übergänge.</p>
        </div>

        <div class="direction-card">
          <h3>Rekursive Zustandsraumerweiterung</h3>
          <p>Systeme, die ihren semantischen Kontext-Raum verfeinern und neu kalibrieren, während Fragen, Informationen und Strukturen wachsen.</p>
        </div>

        <div class="direction-card">
          <h3>Autorensysteme und semantisches Gedächtnis</h3>
          <p>Architekturen für Langform-Schreiben, strukturelles Gedächtnis, rekursives Manuskriptwachstum und perspektivenspezifische Re-Emission desselben Kerns.</p>
        </div>

        <div class="direction-card">
          <h3>Verkörperte Assistenz</h3>
          <p>Zustandssensitive, resonanzbewusste Systeme, die nicht nur reagieren, sondern Timing, Rahmung, Präsenz und semantische Passung modulieren.</p>
        </div>

        <div class="direction-card">
          <h3>Entdeckungssysteme</h3>
          <p>Werkzeuge für Theoriesuche, Fragenerweiterung, Widerspruchsverfolgung und die rekursive Stärkung tragfähiger Erkenntnissuche.</p>
        </div>

        <div class="direction-card">
          <h3>Semantische Sicherheitssysteme</h3>
          <p>Architekturen für Drift-Diagnostik, Interventionssteuerung und kognitive Umgebungen mit mehr Kohärenz, Würde und tragfähigem Handlungsraum.</p>
        </div>
      </div>

      <p class="display-statement wide">
        Diese Richtungen sind keine beliebigen Anwendungsfälle.
        Sie gehen aus derselben zugrunde liegenden Architektur hervor.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="sources-block">
      <h2 class="section-heading-display">Wie man mit diesem Material arbeiten kann</h2>

      <div class="body-copy">
        <ol>
          <li><strong>Einzelne Paper lesen</strong> und auf innere Struktur, formale Kontinuität und Anschlussfähigkeit prüfen.</li>
          <li><strong>Den Sammelband oder die Bundles nutzen</strong>, wenn du einen durchgehenden Zusammenhang statt isolierter Quelleinheiten willst.</li>
          <li><strong>Das Material in dein eigenes KI-System laden</strong>, wenn du Ableitungen, Übergänge, fehlende Spezifikationen und offene Implementierungsfragen systematischer prüfen willst.</li>
        </ol>

        <p>
          In allen drei Fällen sind die nützlichsten Fragen nicht nur,
          ob ein Satz plausibel klingt,
          sondern wie die Struktur gebaut ist:
          welche Begriffe formal eingeführt werden,
          wie die Paper aufeinander aufbauen,
          was bereits gut spezifiziert ist
          und wo empirische oder implementierende Arbeit noch offen bleibt.
        </p>
      </div>

      <div class="status-box">
        <p class="status-label">Lesehaltung</p>
        <p>
          Glaube nicht zu schnell.
          Verwirf nicht zu schnell.
          Lies die Quellenebene,
          verfolge die Struktur
          und prüfe den Rahmen an seinen stärksten Behauptungen.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="sources-next">
      <h2 class="section-heading-display">Nächste Schritte</h2>

      <div class="next-grid">
        <div class="next-card">
          <h3><a href="/de/theorie/">Theorie →</a></h3>
          <p>Das begriffliche und formale Rückgrat in lesbarer Form.</p>
        </div>
        <div class="next-card">
          <h3><a href="/de/ki-alignment/">KI-Alignment →</a></h3>
          <p>Wie der Rahmen zu einer KI-Architektur wird.</p>
        </div>
        <div class="next-card">
          <h3><a href="/de/downloads/">Downloads →</a></h3>
          <p>Gebündelte Prüfungskontexte für direkte Lektüre und KI-gestützte Analyse.</p>
        </div>
        <div class="next-card">
          <h3><a href="/de/implikationen/">Implikationen →</a></h3>
          <p>Was folgt, sobald semantische Struktur operativ wird.</p>
        </div>
      </div>
    </div>
  </section>

</div>
