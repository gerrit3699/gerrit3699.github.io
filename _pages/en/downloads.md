---
layout: default
title: "Downloads"
permalink: /en/downloads/
lang: en
description: "Download bundles, Zenodo papers, and review materials for AI-based analysis, independent reading, and deeper study."
translation_url_de: /de/downloads/
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
      <h1 class="downloads-display">Bundled review material for deeper reading and AI-based examination.</h1>
      <p class="downloads-sublead">
        This page is for <strong>download bundles</strong>.
        These files are meant for larger-context reading, independent review, and especially for loading the material into AI systems as one coherent body.
      </p>

      <div class="body-copy">
        <p>
          If you want the work in its cleanest technical source form, the better route is the individual Zenodo papers on the <strong>Technical Sources</strong> page.
          The bundles here are for a different use:
          not exact source citation first, but larger-context examination.
        </p>

        <p>
          This is also the only page where the <strong>technical applications / application examples</strong> bundle can currently be downloaded in this form.
          That file is a German working document assembled out of the logic of my patent applications and application directions.
          It has not yet been translated into a final English version.
        </p>
      </div>

      <p class="display-statement wide">
        More context does not prove a theory.
        But it changes the mode of review.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="downloads-block">
      <h2 class="section-heading-display">Download bundles</h2>

      <div class="bundle-grid">

        <div class="bundle-card">
          <p class="file-label">Bundle 1</p>
          <h3>Semantic Gravitation I–VI — Collected Papers</h3>

          <div class="bundle-meta">
            <span class="bundle-tag">Collected volume</span>
            <span class="bundle-tag">6 papers in sequence</span>
            <span class="bundle-tag">Best for AI backbone use</span>
          </div>

          <p>
            This is the six-paper backbone in one continuous file.
            It is the strongest bundle here when you want to load the theoretical core into an AI system and question the framework as one larger semantic body.
          </p>

          <p>
            For exact technical reading or citation, the individual Zenodo papers remain the cleaner source route.
          </p>

          <div class="bundle-links">
            <a class="bundle-link" href="/assets/downloads/semantic-gravitation-collected-papers.pdf" download>
              Download collected PDF →
            </a>
            <a class="bundle-link" href="/en/papers/">
              Go to Technical Sources →
            </a>
          </div>
        </div>

        <div class="bundle-card">
          <p class="file-label">Bundle 2</p>
          <h3>Beyond Fog / Edge Alignment bundle</h3>

          <div class="bundle-meta">
            <span class="bundle-tag">Alignment bundle</span>
            <span class="bundle-tag">Paper + patent material</span>
            <span class="bundle-tag">Best for alignment review</span>
          </div>

          <p>
            This bundle combines the alignment paper with related patent material.
            It is useful when you want to work through the broader Edge Alignment logic in one place.
          </p>

          <p>
            For the clean source paper itself, the Zenodo version remains the better route.
          </p>

          <div class="bundle-links">
            <a class="bundle-link" href="/assets/downloads/edge-alignment-paper-patent.pdf" download>
              Download alignment bundle →
            </a>
            <a class="bundle-link" href="https://doi.org/10.5281/zenodo.18608012" target="_blank" rel="noopener">
              Go to the Zenodo paper →
            </a>
          </div>
        </div>

        <div class="bundle-card">
          <p class="file-label">Bundle 3</p>
          <h3>Technical applications / application examples</h3>

          <div class="bundle-meta">
            <span class="bundle-tag">Working document</span>
            <span class="bundle-tag">German only for now</span>
            <span class="bundle-tag">Selected examples</span>
          </div>

          <p>
            This is a selected applications bundle assembled from filings, design principles, and representative system directions.
            It is the place to look when you want a compact view of what kinds of technical applications could emerge from the framework.
          </p>

          <p>
            It is not the full application universe.
            It is a generated working slice for review, and it is currently available only in this German bundled form.
          </p>

          <div class="bundle-links">
            <a class="bundle-link" href="/assets/downloads/semantic-gravitation-anwendungsbeispiele.pdf" download>
              Download applications bundle →
            </a>
            <a class="bundle-link" href="/en/implications/">
              Go to Implications →
            </a>
          </div>
        </div>

      </div>

      <div class="status-box">
        <p class="status-label">Recommended use</p>
        <p>
          Use <strong>Theory</strong> for orientation.
          Use <strong>Technical Sources</strong> for the clean source texts.
          Use these bundles when you want larger coherent files for deeper questioning, reconstruction, or AI-assisted review.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="downloads-next">
      <h2 class="section-heading-display">Next steps</h2>

      <div class="next-grid">
        <div class="next-card">
          <h3><a href="/en/theory/">Theory →</a></h3>
          <p>The best place for orientation before deeper download-based review.</p>
        </div>
        <div class="next-card">
          <h3><a href="/en/alignment/">Alignment →</a></h3>
          <p>The Edge Alignment architecture in web form.</p>
        </div>
        <div class="next-card">
          <h3><a href="/en/papers/">Technical Sources →</a></h3>
          <p>The individual papers and canonical source links.</p>
        </div>
        <div class="next-card">
          <h3><a href="/en/implications/">Implications →</a></h3>
          <p>What follows once the structure becomes operational.</p>
        </div>
      </div>
    </div>
  </section>

</div>
