---
layout: default
title: "Downloads"
permalink: /en/downloads/
lang: en
description: "Download bundles, Zenodo papers, and review materials for AI-based analysis, independent reading, and deeper study."
translation_url_de: /de/downloads/
---

<style>
  html {
    scroll-behavior: smooth;
  }

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
    max-width: 60rem;
    margin: 0 auto 1.2rem;
    font-size: clamp(1.08rem, 2vw, 1.4rem);
    line-height: 1.62;
    text-wrap: balance;
  }

  .downloads-page .claim-grid,
  .downloads-page .bundle-grid,
  .downloads-page .work-grid,
  .downloads-page .next-grid,
  .downloads-page .review-grid {
    display: grid;
    gap: 1rem;
  }

  .downloads-page .claim-grid,
  .downloads-page .work-grid,
  .downloads-page .review-grid {
    grid-template-columns: repeat(3, minmax(0, 1fr));
    max-width: 1080px;
    margin: 1.9rem auto 0;
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

  .downloads-page .claim-card,
  .downloads-page .work-card,
  .downloads-page .review-card,
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

  .downloads-page .claim-card,
  .downloads-page .work-card,
  .downloads-page .review-card,
  .downloads-page .next-card {
    padding: 1.18rem 1rem 1.08rem;
    text-align: center;
  }

  .downloads-page .bundle-card {
    padding: 1.35rem 1.2rem 1.25rem;
    text-align: center;
  }

  .downloads-page .claim-card h3,
  .downloads-page .work-card h3,
  .downloads-page .review-card h3,
  .downloads-page .next-card h3,
  .downloads-page .bundle-card h3 {
    margin: 0 0 0.35rem;
    font-size: 1.18rem;
    line-height: 1.06;
    letter-spacing: -0.03em;
  }

  .downloads-page .bundle-card h3 {
    font-size: 1.34rem;
  }

  .downloads-page .claim-card p,
  .downloads-page .work-card p,
  .downloads-page .review-card p,
  .downloads-page .next-card p,
  .downloads-page .bundle-card p {
    margin: 0;
    font-size: 0.98rem;
    line-height: 1.58;
    color: var(--dl-soft);
  }

  .downloads-page .claim-card {
    display: block;
    text-decoration: none;
    transition:
      transform 0.18s ease,
      border-color 0.18s ease;
  }

  .downloads-page .claim-card:hover {
    transform: translateY(-2px);
    border-color: var(--dl-line-strong);
  }

  .downloads-page .claim-card strong {
    display: block;
    margin-top: 0.75rem;
    font-size: 0.96rem;
    color: #fff;
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

  .downloads-page .body-copy ul,
  .downloads-page .body-copy ol {
    max-width: 42em;
    margin: 1.15rem auto;
    text-align: left;
  }

  .downloads-page .body-copy li {
    margin-bottom: 0.5rem;
  }

  .downloads-page .display-statement {
    max-width: 25ch;
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
  .downloads-page .display-statement.narrow { max-width: 13ch; }

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

  .downloads-page .bundle-link,
  .downloads-page .review-link {
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

  .downloads-page .review-links {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 0.8rem;
    margin-top: 1rem;
  }

  .downloads-page .next-card a {
    color: #fff;
  }

  @media (max-width: 980px) {
    .downloads-page .claim-grid,
    .downloads-page .work-grid,
    .downloads-page .review-grid,
    .downloads-page .next-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="downloads-page">

  <section class="section-shell section-shell-tight">
    <div class="downloads-intro">
      <p class="downloads-kicker">Downloads</p>
      <h1 class="downloads-display">Download bundles for reading, review, and AI-based examination.</h1>
      <p class="downloads-sublead">
        This page is for <strong>bundled review material</strong>.
        If you want the clean technical source texts, use the individual Zenodo papers.
        If you want larger context bodies for AI-assisted questioning, use the bundles here.
      </p>

      <div class="claim-grid">
        <a class="claim-card" href="#direct-technical-reading">
          <h3>Read technically</h3>
          <p>Go to the clean individual papers and source texts.</p>
          <strong>Best: Zenodo papers →</strong>
        </a>
        <a class="claim-card" href="#bundle-downloads">
          <h3>See applications</h3>
          <p>Use the applications bundle for selected technical examples and directions.</p>
          <strong>Best: applications bundle →</strong>
        </a>
        <a class="claim-card" href="#ai-backbone-use">
          <h3>Use as AI backbone</h3>
          <p>Load the collected papers into AI, optionally together with the applications bundle.</p>
          <strong>Best: collected papers →</strong>
        </a>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell" id="direct-technical-reading">
    <div class="downloads-block">
      <h2 class="section-heading-display">What these files are — and what they are not</h2>

      <div class="body-copy">
        <p>
          These bundles are useful because they gather larger parts of the project into coherent review contexts.
          But they are not always the cleanest or most canonical form of the work.
        </p>

        <p>
          If you want to read the work <strong>as precisely and technically as possible</strong>,
          the best route is usually the <strong>individual Zenodo papers</strong> and the source layer on the Technical Sources page.
          The bundles here are primarily there to make larger-context review easier,
          especially with AI.
        </p>
      </div>

      <p class="display-statement wide">
        More context does not prove a theory.
        But it changes the mode of review.
      </p>

      <div class="review-grid">
        <div class="review-card">
          <h3>Best for exact technical reading</h3>
          <p>Use the individual Zenodo papers and the Technical Sources page.</p>
          <div class="review-links">
            <a class="review-link" href="/en/papers/">Go to Technical Sources →</a>
          </div>
        </div>
        <div class="review-card">
          <h3>Best for AI-based reconstruction</h3>
          <p>Use the larger bundles as context bodies and interrogate the system step by step.</p>
          <div class="review-links">
            <a class="review-link" href="#ai-backbone-use">Go to AI backbone use →</a>
          </div>
        </div>
        <div class="review-card">
          <h3>Best for orientation</h3>
          <p>Start with the Theory page, then return here once you know what you want to examine more deeply.</p>
          <div class="review-links">
            <a class="review-link" href="/en/theory/">Go to Theory →</a>
          </div>
        </div>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell" id="bundle-downloads">
    <div class="downloads-block">
      <h2 class="section-heading-display">Download bundles</h2>

      <div class="bundle-grid">

        <div class="bundle-card" id="ai-backbone-use">
          <p class="file-label">Bundle 1</p>
          <h3>Semantic Gravitation I–VI — Collected Papers</h3>

          <div class="bundle-meta">
            <span class="bundle-tag">Collected volume</span>
            <span class="bundle-tag">6 papers in sequence</span>
            <span class="bundle-tag">Best for AI backbone use</span>
          </div>

          <p>
            This is a <strong>single collected document</strong> in which all six papers are placed one after another.
            It is most useful when you want the whole theoretical backbone in one coherent file,
            especially as a context body for AI-assisted reconstruction.
          </p>

          <p>
            If your goal is to <strong>use the system with AI and ask it deeper questions</strong>,
            this is usually the central file to load first.
            In many cases it also makes sense to add the <strong>applications bundle</strong> alongside it,
            because that gives the AI not only the formal backbone,
            but also selected system directions and examples.
          </p>

          <p>
            It is <strong>not better than the individual Zenodo papers</strong> as a canonical source.
            If you want to read, cite, or inspect the papers one by one,
            the individual Zenodo entries are the cleaner route.
          </p>

          <div class="bundle-links">
            <a class="bundle-link" href="/assets/downloads/semantic-gravitation-collected-papers.pdf" download>
              Download collected PDF →
            </a>
            <a class="bundle-link" href="/en/papers/">
              Go to Technical Sources / Zenodo links →
            </a>
          </div>
        </div>

        <div class="bundle-card">
          <p class="file-label">Bundle 2</p>
          <h3>Beyond Fog / Edge Alignment bundle</h3>

          <div class="bundle-meta">
            <span class="bundle-tag">Combined bundle</span>
            <span class="bundle-tag">Paper + patent material</span>
            <span class="bundle-tag">Best for alignment-specific review</span>
          </div>

          <p>
            This file is a <strong>combined alignment bundle</strong>.
            It brings together the alignment paper and the related patent material in one place.
            That makes it useful when you want to work through the broader Edge Alignment logic with AI.
          </p>

          <p>
            It is <strong>not a perfectly cleaned standalone edition</strong>.
            If you want the clean source version of the alignment paper itself,
            it is better to go directly to the Zenodo paper
            <strong>Beyond Fog: Edge Alignment in Semantic Space</strong>.
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

        <div class="bundle-card" id="applications-bundle">
          <p class="file-label">Bundle 3</p>
          <h3>Technical applications / application examples</h3>

          <div class="bundle-meta">
            <span class="bundle-tag">Generated working document</span>
            <span class="bundle-tag">Selected examples only</span>
            <span class="bundle-tag">Best for application lines</span>
          </div>

          <p>
            This file is a <strong>generated working document</strong> assembled from patent filings,
            design principles, and selected application examples.
            It is not the full application universe.
            It is a representative slice of a much larger body of technical directions.
          </p>

          <p>
            If you want to <strong>see application examples and system directions</strong>,
            this is the right bundle.
            It is not meant as a final catalog.
            It is meant as a workable review body for asking:
            what kinds of systems, products, and architectures could actually emerge from this framework?
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
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="downloads-block">
      <h2 class="section-heading-display">How to use these bundles well</h2>

      <div class="work-grid">
        <div class="work-card">
          <h3>Ask structural questions</h3>
          <p>Do the concepts cohere? Are the transitions clean? Where does the architecture begin to hold?</p>
        </div>
        <div class="work-card">
          <h3>Separate core from frontier</h3>
          <p>Which parts look theoretically strong already? Which parts remain open, speculative, or still under development?</p>
        </div>
        <div class="work-card">
          <h3>Push toward implementation</h3>
          <p>What would need to be formalized, modeled, benchmarked, or engineered to turn these ideas into robust systems?</p>
        </div>
      </div>

      <p class="display-statement medium">
        Do not believe too quickly.
        Do not reject too quickly.
        Examine carefully.
      </p>

      <div class="body-copy">
        <p>
          The most useful method is usually not to react to a few isolated quotations,
          but to give an AI system a larger coherent document
          and then ask sharper questions about terms, transitions, assumptions, tensions, and implementability.
        </p>

        <p>
          For that purpose, it matters much less whether a source is in English or German.
          For an AI system, both can function as usable context for reconstructing the principles.
        </p>
      </div>

      <div class="status-box">
        <p class="status-label">Recommended workflow</p>
        <p>
          Use the Theory page for orientation.
          Use the Zenodo papers for the clean technical source texts.
          Use the collected papers — optionally together with the applications bundle — when you want an AI-readable backbone for deeper questioning.
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
          <p>The formal backbone behind the documents.</p>
        </div>
        <div class="next-card">
          <h3><a href="/en/alignment/">Alignment →</a></h3>
          <p>The Edge Alignment architecture in web form.</p>
        </div>
        <div class="next-card">
          <h3><a href="/en/papers/">Technical Sources →</a></h3>
          <p>The individual papers and source links.</p>
        </div>
        <div class="next-card">
          <h3><a href="/en/implications/">Implications →</a></h3>
          <p>What follows once the structure becomes operational.</p>
        </div>
      </div>
    </div>
  </section>

</div>
