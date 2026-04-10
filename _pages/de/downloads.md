---
layout: default
title: "Downloads"
permalink: /de/downloads/
lang: de
description: "Download-Bundles, Zenodo-Paper und Prüfmaterialien für KI-gestützte Analyse, eigenständige Lektüre und vertiefte Prüfung."
translation_url_en: /en/downloads/
---

<style>
  .downloads-page {
    --dl-text: rgba(255,255,255,0.96);
    --dl-soft: rgba(255,255,255,0.82);
    --dl-faint: rgba(255,255,255,0.64);
    --dl-line: rgba(255,255,255,0.10);
    --dl-line-strong: rgba(255,255,255,0.16);
  }

  .downloads-page h1,
  .downloads-page h2,
  .downloads-page h3,
  .downloads-page strong,
  .downloads-page a {
    color: #fff;
  }

  .downloads-page p,
  .downloads-page li {
    color: var(--dl-text);
  }

  .downloads-page .section-shell {
    padding-top: 2.8rem;
    padding-bottom: 2.8rem;
  }

  .downloads-page .section-shell-tight {
    padding-top: 2.1rem;
    padding-bottom: 2.1rem;
  }

  .downloads-page .downloads-intro,
  .downloads-page .downloads-block,
  .downloads-page .downloads-next {
    max-width: 1080px;
    margin: 0 auto;
  }

  .downloads-page .downloads-intro,
  .downloads-page .body-copy,
  .downloads-page .downloads-next {
    text-align: center;
  }

  .downloads-page .downloads-kicker,
  .downloads-page .status-label,
  .downloads-page .file-label {
    margin: 0 0 0.7rem;
    font-size: 0.88rem;
    letter-spacing: 0.16em;
    text-transform: uppercase;
    color: var(--dl-faint);
  }

  .downloads-page .downloads-display {
    margin: 0 auto 1.15rem;
    max-width: 11ch;
    font-size: clamp(2.5rem, 6vw, 5rem);
    line-height: 0.94;
    letter-spacing: -0.05em;
    font-weight: 650;
    text-wrap: balance;
  }

  .downloads-page .downloads-sublead {
    max-width: 58rem;
    margin: 0 auto 1.2rem;
    font-size: clamp(1.08rem, 2vw, 1.4rem);
    line-height: 1.62;
    text-wrap: balance;
  }

  .downloads-page .section-heading-display {
    margin: 0 auto 1.3rem;
    max-width: 14ch;
    text-align: center;
    font-size: clamp(2.05rem, 4.8vw, 3.7rem);
    line-height: 0.98;
    letter-spacing: -0.045em;
    text-wrap: balance;
  }

  .downloads-page .body-copy {
    max-width: 940px;
    margin: 0 auto;
  }

  .downloads-page .body-copy p {
    max-width: 46em;
    margin: 0.95rem auto 0;
    font-size: 1.1rem;
    line-height: 1.76;
    letter-spacing: -0.01em;
  }

  .downloads-page .display-statement {
    max-width: 24ch;
    margin: 1.9rem auto;
    text-align: center;
    font-size: clamp(1.9rem, 3.6vw, 3rem);
    line-height: 1.03;
    letter-spacing: -0.045em;
    font-weight: 650;
    text-wrap: balance;
  }

  .downloads-page .display-statement.wide { max-width: 30ch; }
  .downloads-page .display-statement.medium { max-width: 22ch; }

  .downloads-page .bundle-grid,
  .downloads-page .next-grid {
    display: grid;
    gap: 1rem;
  }

  .downloads-page .bundle-grid {
    grid-template-columns: 1fr;
    max-width: 980px;
    margin: 1.9rem auto 0;
  }

  .downloads-page .next-grid {
    grid-template-columns: repeat(4, minmax(0, 1fr));
    max-width: 1080px;
    margin: 1.8rem auto 0;
  }

  .downloads-page .bundle-card,
  .downloads-page .next-card,
  .downloads-page .status-box {
    border: 1px solid var(--dl-line);
    border-radius: 22px;
    background: linear-gradient(180deg, rgba(255,255,255,0.05), rgba(255,255,255,0.025));
    box-shadow:
      0 18px 48px rgba(0,0,0,0.18),
      inset 0 1px 0 rgba(255,255,255,0.03);
  }

  .downloads-page .next-card {
    padding: 1.18rem 1rem 1.08rem;
    text-align: center;
  }

  .downloads-page .bundle-card {
    padding: 1.35rem 1.2rem 1.25rem;
    text-align: center;
  }

  .downloads-page .next-card h3,
  .downloads-page .bundle-card h3 {
    margin: 0 0 0.35rem;
    font-size: 1.18rem;
    line-height: 1.08;
    letter-spacing: -0.03em;
  }

  .downloads-page .bundle-card h3 {
    font-size: 1.34rem;
  }

  .downloads-page .next-card p,
  .downloads-page .bundle-card p {
    margin: 0;
    font-size: 0.98rem;
    line-height: 1.58;
    color: var(--dl-soft);
  }

  .downloads-page .bundle-meta {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 0.6rem;
    margin: 0.9rem 0 1rem;
  }

  .downloads-page .bundle-tag {
    display: inline-flex;
    align-items: center;
    min-height: 34px;
    padding: 0.45rem 0.75rem;
    border-radius: 999px;
    border: 1px solid var(--dl-line);
    background: rgba(255,255,255,0.04);
    font-size: 0.88rem;
    line-height: 1.2;
    color: var(--dl-soft);
  }

  .downloads-page .bundle-links {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 0.8rem;
    margin-top: 1.2rem;
  }

  .downloads-page .bundle-link {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 46px;
    padding: 0.85rem 1.05rem;
    border-radius: 999px;
    border: 1px solid var(--dl-line);
    background: rgba(255,255,255,0.04);
    text-decoration: none;
    font-size: 0.96rem;
    line-height: 1.2;
  }

  .downloads-page .status-box {
    max-width: 920px;
    margin: 2rem auto 0;
    padding: 1.2rem 1.15rem;
    text-align: center;
  }

  .downloads-page .status-box p {
    margin: 0;
    font-size: clamp(1.16rem, 2.2vw, 1.68rem);
    line-height: 1.38;
    text-wrap: balance;
  }

  .downloads-page .next-card a {
    color: #fff;
  }

  @media (max-width: 980px) {
    .downloads-page .next-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="downloads-page">

  <section class="section-shell section-shell-tight">
    <div class="downloads-intro">
      <p class="downloads-kicker">Downloads</p>
      <h1 class="downloads-display">Gebündeltes Prüfmaterial für vertiefte Lektüre und KI-gestützte Untersuchung.</h1>
      <p class="downloads-sublead">
        Diese Seite ist für <strong>Download-Bundles</strong>.
        Die Dateien sind für Lektüre im größeren Zusammenhang,
        eigenständige Prüfung
        und besonders dafür gedacht,
        das Material als zusammenhängenden Körper in KI-Systeme zu laden.
      </p>

      <div class="body-copy">
        <p>
          Wenn du die Arbeit in ihrer saubersten technischen Quellenform lesen willst,
          ist der bessere Weg die einzelne Zenodo-Veröffentlichung auf der Seite
          <strong>Technische Quellen</strong>.
          Die Bundles hier dienen einem anderen Zweck:
          nicht zuerst exakter Quellenzitation,
          sondern Prüfung im größeren Zusammenhang.
        </p>

        <p>
          Das ist zugleich die einzige Seite,
          auf der das Bundle <strong>Technische Anwendungen / Anwendungsbeispiele</strong>
          derzeit in dieser Form heruntergeladen werden kann.
          Diese Datei ist ein deutschsprachiges Arbeitsdokument,
          das aus der Logik meiner Patentanmeldungen und Anwendungsrichtungen heraus zusammengestellt wurde.
          Eine finale englische Fassung existiert dafür bisher noch nicht.
        </p>
      </div>

      <p class="display-statement wide">
        Mehr Kontext beweist keine Theorie.
        Aber er verändert die Art ihrer Prüfung.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="downloads-block">
      <h2 class="section-heading-display">Download-Bundles</h2>

      <div class="bundle-grid">

        <div class="bundle-card">
          <p class="file-label">Bundle 1</p>
          <h3>Semantic Gravitation I–VI — Collected Papers</h3>

          <div class="bundle-meta">
            <span class="bundle-tag">Gesamtband</span>
            <span class="bundle-tag">6 Paper in Folge</span>
            <span class="bundle-tag">Am besten als KI-Backbone</span>
          </div>

          <p>
            Das ist das Rückgrat aus sechs Papern in einer durchgehenden Datei.
            Es ist hier das stärkste Bundle,
            wenn du den theoretischen Kern in ein KI-System laden
            und den Rahmen als einen größeren semantischen Zusammenhang befragen willst.
          </p>

          <p>
            Für exakte technische Lektüre oder Zitation
            bleiben die einzelnen Zenodo-Paper der sauberere Quellenweg.
          </p>

          <div class="bundle-links">
            <a class="bundle-link" href="/assets/downloads/semantic-gravitation-collected-papers.pdf" download>
              Gesamt-PDF herunterladen →
            </a>
            <a class="bundle-link" href="/de/papers/">
              Zu den technischen Quellen →
            </a>
          </div>
        </div>

        <div class="bundle-card">
          <p class="file-label">Bundle 2</p>
          <h3>Beyond Fog / Edge Alignment bundle</h3>

          <div class="bundle-meta">
            <span class="bundle-tag">Alignment-Bundle</span>
            <span class="bundle-tag">Paper + Patentmaterial</span>
            <span class="bundle-tag">Am besten für Alignment-Prüfung</span>
          </div>

          <p>
            Dieses Bundle verbindet das Alignment-Paper
            mit zugehörigem Patentmaterial.
            Es ist nützlich,
            wenn du die breitere Logik von Edge Alignment an einem Ort durcharbeiten willst.
          </p>

          <p>
            Für das saubere Quellenpaper selbst
            bleibt die Zenodo-Version der bessere Weg.
          </p>

          <div class="bundle-links">
            <a class="bundle-link" href="/assets/downloads/edge-alignment-paper-patent.pdf" download>
              Alignment-Bundle herunterladen →
            </a>
            <a class="bundle-link" href="https://doi.org/10.5281/zenodo.18608012" target="_blank" rel="noopener">
              Zum Zenodo-Paper →
            </a>
          </div>
        </div>

        <div class="bundle-card">
          <p class="file-label">Bundle 3</p>
          <h3>Technische Anwendungen / Anwendungsbeispiele</h3>

          <div class="bundle-meta">
            <span class="bundle-tag">Arbeitsdokument</span>
            <span class="bundle-tag">Derzeit nur auf Deutsch</span>
            <span class="bundle-tag">Ausgewählte Beispiele</span>
          </div>

          <p>
            Das ist ein ausgewähltes Anwendungs-Bundle,
            zusammengestellt aus Einreichungen,
            Designprinzipien
            und repräsentativen Systemrichtungen.
            Hier findest du in kompakter Form,
            welche technischen Anwendungen aus dem Rahmen hervorgehen könnten.
          </p>

          <p>
            Es ist nicht das vollständige Anwendungsuniversum.
            Es ist ein erzeugter Arbeitsausschnitt für Prüfung und weitere Befragung
            und liegt derzeit nur in dieser gebündelten deutschen Form vor.
          </p>

          <div class="bundle-links">
            <a class="bundle-link" href="/assets/downloads/semantic-gravitation-anwendungsbeispiele.pdf" download>
              Anwendungs-Bundle herunterladen →
            </a>
            <a class="bundle-link" href="/de/implikationen/">
              Zu den Implikationen →
            </a>
          </div>
        </div>

      </div>

      <div class="status-box">
        <p class="status-label">Empfohlene Nutzung</p>
        <p>
          Nutze <strong>Theorie</strong> zur Orientierung.
          Nutze <strong>Technische Quellen</strong> für die sauberen Quellentexte.
          Nutze diese Bundles,
          wenn du größere zusammenhängende Dateien
          für vertiefte Befragung,
          Rekonstruktion
          oder KI-gestützte Prüfung haben willst.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="downloads-next">
      <h2 class="section-heading-display">Nächste Schritte</h2>

      <div class="next-grid">
        <div class="next-card">
          <h3><a href="/de/theorie/">Theorie →</a></h3>
          <p>Der beste Ort zur Orientierung vor tieferer prüfender Lektüre über Downloads.</p>
        </div>
        <div class="next-card">
          <h3><a href="/de/ki-alignment/">KI-Alignment →</a></h3>
          <p>Die Edge-Alignment-Architektur in Webform.</p>
        </div>
        <div class="next-card">
          <h3><a href="/de/papers/">Technische Quellen →</a></h3>
          <p>Die einzelnen Paper und kanonischen Quellenlinks.</p>
        </div>
        <div class="next-card">
          <h3><a href="/de/implikationen/">Implikationen →</a></h3>
          <p>Was folgt, sobald die Struktur operativ wird.</p>
        </div>
      </div>
    </div>
  </section>

</div>
