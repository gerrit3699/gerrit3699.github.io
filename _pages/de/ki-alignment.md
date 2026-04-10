---
layout: default
title: KI-Alignment
permalink: /de/ki-alignment/
lang: de
description: "Edge Alignment als Architektur semantischer Navigation: von Antwortsystemen zu tragfähig ausgerichteten KI-Systemen."
translation_url_en: /en/alignment/
---

<style>
  .alignment-page {
    --align-text: rgba(255,255,255,0.96);
    --align-soft: rgba(255,255,255,0.82);
    --align-faint: rgba(255,255,255,0.64);
    --align-line: rgba(255,255,255,0.10);
    --align-line-strong: rgba(255,255,255,0.16);
  }

  .alignment-page h1,
  .alignment-page h2,
  .alignment-page h3,
  .alignment-page strong,
  .alignment-page a {
    color: #fff;
  }

  .alignment-page p,
  .alignment-page li {
    color: var(--align-text);
  }

  .alignment-page .section-shell {
    padding-top: 2.8rem;
    padding-bottom: 2.8rem;
  }

  .alignment-page .section-shell-tight {
    padding-top: 2.1rem;
    padding-bottom: 2.1rem;
  }

  .alignment-page .align-intro,
  .alignment-page .align-block,
  .alignment-page .align-next {
    max-width: 1080px;
    margin: 0 auto;
  }

  .alignment-page .align-intro,
  .alignment-page .body-copy,
  .alignment-page .closing-block,
  .alignment-page .align-next {
    text-align: center;
  }

  .alignment-page .align-kicker,
  .alignment-page .status-label {
    margin: 0 0 0.7rem;
    font-size: 0.88rem;
    letter-spacing: 0.16em;
    text-transform: uppercase;
    color: var(--align-faint);
  }

  .alignment-page .align-display {
    margin: 0 auto 1.15rem;
    max-width: 12ch;
    font-size: clamp(2.5rem, 6vw, 5.1rem);
    line-height: 0.94;
    letter-spacing: -0.05em;
    font-weight: 650;
    text-wrap: balance;
  }

  .alignment-page .align-sublead {
    max-width: 58rem;
    margin: 0 auto 1.2rem;
    font-size: clamp(1.08rem, 2vw, 1.4rem);
    line-height: 1.62;
    text-wrap: balance;
  }

  .alignment-page .claim-grid,
  .alignment-page .concept-grid,
  .alignment-page .capability-grid,
  .alignment-page .next-grid,
  .alignment-page .compare-grid,
  .alignment-page .system-grid {
    display: grid;
    gap: 1rem;
  }

  .alignment-page .claim-grid,
  .alignment-page .concept-grid,
  .alignment-page .capability-grid,
  .alignment-page .system-grid {
    grid-template-columns: repeat(3, minmax(0, 1fr));
    max-width: 1080px;
    margin: 1.9rem auto 0;
  }

  .alignment-page .compare-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
    max-width: 960px;
    margin: 1.9rem auto 0;
  }

  .alignment-page .next-grid {
    grid-template-columns: repeat(4, minmax(0, 1fr));
    max-width: 1080px;
    margin: 1.8rem auto 0;
  }

  .alignment-page .claim-card,
  .alignment-page .concept-card,
  .alignment-page .capability-card,
  .alignment-page .system-card,
  .alignment-page .compare-card,
  .alignment-page .next-card,
  .alignment-page .status-box {
    border: 1px solid var(--align-line);
    border-radius: 22px;
    background: linear-gradient(180deg, rgba(255,255,255,0.05), rgba(255,255,255,0.025));
    box-shadow:
      0 18px 48px rgba(0,0,0,0.18),
      inset 0 1px 0 rgba(255,255,255,0.03);
  }

  .alignment-page .claim-card,
  .alignment-page .concept-card,
  .alignment-page .capability-card,
  .alignment-page .system-card,
  .alignment-page .compare-card,
  .alignment-page .next-card {
    padding: 1.18rem 1rem 1.08rem;
    text-align: center;
  }

  .alignment-page .claim-card h3,
  .alignment-page .concept-card h3,
  .alignment-page .capability-card h3,
  .alignment-page .system-card h3,
  .alignment-page .compare-card h3,
  .alignment-page .next-card h3 {
    margin: 0 0 0.35rem;
    font-size: 1.18rem;
    line-height: 1.06;
    letter-spacing: -0.03em;
  }

  .alignment-page .claim-card p,
  .alignment-page .concept-card p,
  .alignment-page .capability-card p,
  .alignment-page .system-card p,
  .alignment-page .compare-card p,
  .alignment-page .next-card p {
    margin: 0;
    font-size: 0.98rem;
    line-height: 1.54;
    color: var(--align-soft);
  }

  .alignment-page .section-heading-display {
    margin: 0 auto 1.3rem;
    max-width: 14ch;
    text-align: center;
    font-size: clamp(2.05rem, 4.8vw, 3.7rem);
    line-height: 0.98;
    letter-spacing: -0.045em;
    text-wrap: balance;
  }

  .alignment-page .body-copy {
    max-width: 940px;
    margin: 0 auto;
  }

  .alignment-page .body-copy p {
    max-width: 46em;
    margin: 0.95rem auto 0;
    font-size: 1.1rem;
    line-height: 1.76;
    letter-spacing: -0.01em;
  }

  .alignment-page .body-copy ul,
  .alignment-page .body-copy ol {
    max-width: 42em;
    margin: 1.15rem auto;
    text-align: left;
  }

  .alignment-page .body-copy li {
    margin-bottom: 0.5rem;
  }

  .alignment-page .display-statement {
    max-width: 25ch;
    margin: 1.9rem auto;
    text-align: center;
    font-size: clamp(1.9rem, 3.6vw, 3rem);
    line-height: 1.03;
    letter-spacing: -0.045em;
    font-weight: 650;
    text-wrap: balance;
  }

  .alignment-page .display-statement.wide { max-width: 30ch; }
  .alignment-page .display-statement.medium { max-width: 22ch; }
  .alignment-page .display-statement.narrow { max-width: 12ch; }

  .alignment-page .status-box {
    max-width: 920px;
    margin: 2rem auto 0;
    padding: 1.2rem 1.15rem;
    text-align: center;
  }

  .alignment-page .status-box p {
    margin: 0;
    font-size: clamp(1.18rem, 2.2vw, 1.7rem);
    line-height: 1.38;
    text-wrap: balance;
  }

  .alignment-page .review-links {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 0.8rem;
    margin-top: 1rem;
  }

  .alignment-page .review-link {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 46px;
    padding: 0.85rem 1.05rem;
    border-radius: 999px;
    border: 1px solid var(--align-line);
    background: rgba(255,255,255,0.04);
    text-decoration: none;
    font-size: 0.96rem;
    line-height: 1.2;
  }

  .alignment-page .next-card a {
    color: #fff;
  }

  @media (max-width: 980px) {
    .alignment-page .claim-grid,
    .alignment-page .concept-grid,
    .alignment-page .capability-grid,
    .alignment-page .system-grid,
    .alignment-page .compare-grid,
    .alignment-page .next-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="alignment-page">

  <section class="section-shell section-shell-tight">
    <div class="align-intro">
      <p class="align-kicker">KI-Alignment</p>
      <h1 class="align-display">KI braucht nicht nur bessere Antworten. Sie braucht bessere innere Wege.</h1>
      <p class="align-sublead">
        Edge Alignment versteht Alignment nicht als nachträglichen Filter auf Ausgaben,
        sondern als Navigation durch semantischen Raum.
        Die eigentliche Frage ist nicht nur, ob eine Antwort akzeptabel aussieht.
        Sie lautet: <strong>Auf welchem Bedeutungsweg ist das System dort hingelangt?</strong>
      </p>

      <div class="claim-grid">
        <div class="claim-card">
          <h3>Nicht nur Ausgaben</h3>
          <p>Alignment muss auf den Weg schauen, nicht nur auf den letzten Satz.</p>
        </div>
        <div class="claim-card">
          <h3>Nicht nur Sicherheit</h3>
          <p>Entscheidend ist, ob der Denkraum tragfähig bleibt, nicht nur regelkonform.</p>
        </div>
        <div class="claim-card">
          <h3>Nicht nur Verhalten</h3>
          <p>Die tiefere Aufgabe ist semantische Navigation, Diagnostik und Reparierbarkeit.</p>
        </div>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="align-block">
      <h2 class="section-heading-display">Was an den meisten heutigen Alignment-Ansätzen falsch läuft</h2>

      <div class="body-copy">
        <p>
          Die meisten heutigen Alignment-Ansätze fragen,
          ob eine Antwort sicher genug,
          hilfreich genug,
          harmlos genug
          oder nah genug an einer Nutzerpräferenz ist.
          Das ist nicht unwichtig.
          Aber es greift spät in den Prozess ein.
        </p>

        <p>
          Ein System kann höflich klingen
          und trotzdem einen schlechten semantischen Pfad durchlaufen.
          Es kann Widerspruch glätten, statt ihn wirklich zu bearbeiten.
          Es kann Unsicherheit kaschieren, statt sie ehrlich zu tragen.
          Es kann Fürsorge simulieren und dabei still den Raum des Denkens verengen.
        </p>
      </div>

      <p class="display-statement wide">
        Ein System ist nicht schon gut ausgerichtet,
        weil seine Antworten gut klingen.
        Es ist ausgerichtet,
        wenn seine inneren semantischen Übergänge tragfähig sind.
      </p>

      <div class="compare-grid">
        <div class="compare-card">
          <h3>Typisches Alignment</h3>
          <p>Riskante Ausgaben blockieren. Akzeptable Antworten belohnen. Die sichtbare Oberfläche glätten.</p>
        </div>
        <div class="compare-card">
          <h3>Edge Alignment</h3>
          <p>Den semantischen Zustand lesen. Drift verfolgen. Tragfähige Fortsetzungen offenhalten. Den Pfad reparieren.</p>
        </div>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="align-block">
      <h2 class="section-heading-display">Der eigentliche architektonische Sprung</h2>

      <div class="body-copy">
        <p>
          Wenn Bedeutung ein Raum ist,
          dann ist Alignment nicht länger nur Regelsetzung für Antworten.
          Dann wird es zu Navigation in diesem Raum.
        </p>

        <p>
          Das verändert das Problem vollständig.
          Die Aufgabe ist nicht mehr nur,
          den richtigen Satz zu erzeugen.
          Die Aufgabe ist,
          semantische Zustände zu erkennen,
          Spannungen zu lokalisieren,
          lokale Entlastung von tieferer Kohärenz zu unterscheiden
          und den nächsten tragfähigen Schritt zu finden.
        </p>
      </div>

      <p class="display-statement medium">
        Alignment verschiebt sich
        von Antwortkontrolle
        zu semantischer Navigation.
      </p>

      <div class="capability-grid">
        <div class="capability-card">
          <h3>Zustände lesen</h3>
          <p>Wo steht das Gespräch strukturell gerade?</p>
        </div>
        <div class="capability-card">
          <h3>Bewegung verfolgen</h3>
          <p>Klärt das System, driftet es, kollabiert es oder öffnet es den Raum?</p>
        </div>
        <div class="capability-card">
          <h3>Übergänge wählen</h3>
          <p>Welcher nächste Schritt erhöht Tragfähigkeit, statt nur die Oberfläche zu glätten?</p>
        </div>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="align-block">
      <h2 class="section-heading-display">Was sich in wiederholter Arbeit gezeigt hat</h2>

      <div class="body-copy">
        <p>
          Das Kernproblem wird sichtbar,
          sobald Antwortqualität als ganze Geschichte behandelt wird.
          In der wiederholten Arbeit mit KI zeigte sich ein Muster:
          Antworten wirkten oft überzeugend
          nicht deshalb, weil sie tiefer wahr waren,
          sondern weil sie den Raum zu früh schlossen.
        </p>

        <p>
          Dadurch verschiebt sich der Fokus.
          Die entscheidenden Fragen werden:
          Welche Frage öffnet einen Raum?
          Welche verengt ihn?
          Was erzeugt wirkliche Klarheit statt glatterer Verwirrung?
          Wann wird ein Widerspruch wirklich durchgearbeitet
          und wann nur eleganter überdeckt?
        </p>
      </div>

      <p class="display-statement medium">
        Das verborgene Problem
        sind nicht nur schlechte Antworten.
        Es ist der vorschnelle Abschluss semantischen Raums.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="align-block">
      <h2 class="section-heading-display">Minimale semantische Ebene</h2>

      <div class="body-copy">
        <p>
          Jede Alignment-Architektur,
          die unterhalb der Oberfläche arbeiten will,
          braucht eine explizite semantische Ebene.
          Der erste minimale Kandidat dafür ist KPR.
        </p>
      </div>

      <div class="concept-grid">
        <div class="concept-card">
          <h3>Kern</h3>
          <p>Worum es in Wahrheit geht.</p>
        </div>
        <div class="concept-card">
          <h3>Projektion</h3>
          <p>Wie es in Sprache, Verhalten, Rahmung oder Signal erscheint.</p>
        </div>
        <div class="concept-card">
          <h3>Relation</h3>
          <p>Womit es verbunden ist und wie diese Verbindungen tragen.</p>
        </div>
      </div>

      <div class="body-copy">
        <p>
          Ein System,
          das nur auf Oberflächenformulierungen reagiert,
          reagiert vor allem auf Projektion.
          Ein tiefer ausgerichtetes System
          muss Kern und Relation mitlesen können.
        </p>

        <p>
          Genau das macht aus bloßer Verhaltenssteuerung
          eine semantische Architektur.
        </p>
      </div>

      <p class="display-statement medium">
        Ohne eine explizite Grammatik der Bedeutung
        bleibt Alignment flach.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="align-block">
      <h2 class="section-heading-display">Operative Achsen der Navigation</h2>

      <div class="body-copy">
        <p>
          KPR liefert die minimale Struktur.
          Ein ausgerichtetes System braucht aber auch eine Weise zu lesen,
          ob Bewegung in einem Raum tragfähiger oder untragfähiger wird.
        </p>

        <p>
          Dafür sind drei operative Achsen entscheidend.
          In den formaler ausgearbeiteten Papern erscheinen sie als
          <strong>Kohärenz, Bindung und Handlungsfähigkeit</strong>.
          Auf der menschlich lesbaren Ebene
          lassen sie sich auch als
          <strong>Klarheit, Würde und Freiheit</strong> lesen.
        </p>
      </div>

      <div class="concept-grid">
        <div class="concept-card">
          <h3>Kohärenz (Klarheit)</h3>
          <p>Macht das System Unterscheidungen lesbarer oder nur glatter?</p>
        </div>
        <div class="concept-card">
          <h3>Bindung (Würde)</h3>
          <p>Bleibt Relation tragfähig, oder wird Entlastung auf Kosten von Wahrheit und menschlichem Stand erkauft?</p>
        </div>
        <div class="concept-card">
          <h3>Handlungsfähigkeit (Freiheit)</h3>
          <p>Bleiben wirkliche Ausdrucks- und Handlungsmöglichkeiten offen, oder werden sie still verengt?</p>
        </div>
      </div>

      <p class="display-statement medium">
        Die Frage lautet nicht nur:
        „Ist diese Antwort okay?“
        Sondern:
        „Was macht dieser Schritt mit der Tragfähigkeit des Raums?“
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="align-block">
      <h2 class="section-heading-display">Die Edge und die Reparierbarkeit</h2>

      <div class="body-copy">
        <p>
          Sobald semantische Bewegung ernst genommen wird,
          wird ein Prinzip zentral:
          Gute Veränderung sollte über minimale,
          verständliche,
          reparierbare Übergänge geschehen.
        </p>

        <p>
          Nicht drei Umdeutungen auf einmal.
          Nicht ein lokaler Gewinn,
          der anderswo still Bindung oder Handlungsfähigkeit zerstört.
          Keine verborgenen Sprünge,
          die Korrektur unmöglich machen.
        </p>
      </div>

      <p class="display-statement narrow">
        Ein Schritt.
        Eine Achse.
        Reparierbar.
      </p>

      <div class="body-copy">
        <p>
          Das ist die Logik der Edge.
          Sie ist keine Stilvorliebe.
          Sie ist Steuerlogik.
        </p>

        <p>
          Ein tragfähiges System darf sich nicht nur bewegen.
          Es muss sich so bewegen,
          dass Korrektur möglich bleibt.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="align-block">
      <h2 class="section-heading-display">Warum sich das tatsächlich bauen lässt</h2>

      <div class="body-copy">
        <p>
          Das ist nicht nur attraktive Sprache.
          Es lässt sich in maschinelle Begriffe übersetzen.
        </p>

        <p>
          Prinzipiell können Systeme darauf trainiert werden,
          Kerne zu identifizieren,
          Projektionen zu unterscheiden,
          Relationen zu gewichten,
          Widerspruchsdruck zu schätzen,
          Drift zu verfolgen
          und alternative Übergänge miteinander zu vergleichen.
        </p>

        <p>
          Sobald das möglich wird,
          ist Bedeutung nicht länger nur eine Wolke um die Ausgabe herum.
          Sie wird zu einem operativen Raum.
        </p>
      </div>

      <p class="display-statement wide">
        Sobald tragfähige semantische Bewegung modellierbar wird,
        hört Alignment auf,
        nur moralische Filterung zu sein,
        und wird zu Ingenieurarbeit.
      </p>

      <div class="capability-grid">
        <div class="capability-card">
          <h3>Semantische Diagnostik</h3>
          <p>Widerspruch, Nebel, Kollapsdruck und Drift lesen.</p>
        </div>
        <div class="capability-card">
          <h3>Übergangssimulation</h3>
          <p>Mögliche nächste Schritte vergleichen, bevor das System auf eine Antwort kollabiert.</p>
        </div>
        <div class="capability-card">
          <h3>Pfadkontrolle</h3>
          <p>Auf tragfähige Bewegung optimieren, nicht nur auf akzeptable Formulierungen.</p>
        </div>
      </div>

      <div class="status-box">
        <p class="status-label">Prüfmaterial</p>
        <p>
          Dieses Alignment-Modell wird hier nicht nur im Fließtext beschrieben.
          Es ist auch auf der <strong>Downloads</strong>-Seite
          und in den <strong>Technischen Quellen</strong> weiter ausgearbeitet.
        </p>
        <div class="review-links">
          <a class="review-link" href="/de/downloads/">Zu den Downloads →</a>
          <a class="review-link" href="/de/papers/">Zu den technischen Quellen →</a>
        </div>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="align-block">
      <h2 class="section-heading-display">Der Scanner semantischer Räume</h2>

      <div class="body-copy">
        <p>
          Die größere Konsequenz ist ein neuer Systemtyp:
          nicht nur ein Chatbot,
          nicht nur eine Antwortmaschine,
          sondern etwas,
          das eher einem <strong>Scanner semantischer Räume</strong> entspricht.
        </p>

        <p>
          Ein solches System würde nicht bloß antworten.
          Es würde sichtbar machen,
          wo sich ein Raum verengt,
          wo Widerspruch nur kosmetisch verdeckt wird,
          wo zwei Positionen nur lokal gegensätzlich erscheinen
          und welcher nächste Schritt die Tragfähigkeit tatsächlich erhöht.
        </p>
      </div>

      <p class="display-statement medium">
        Ein Scanner semantischer Räume
        würde nicht bloß Ausgaben bewerten.
        Er würde Zustände und Übergänge lesen.
      </p>

      <div class="status-box">
        <p class="status-label">Architektonische Konsequenz</p>
        <p>
          Das ist kein kleines Upgrade heutiger KI.
          Es ist eine neue Architekturklasse.
        </p>
      </div>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="align-block">
      <h2 class="section-heading-display">Welche neuen Systemtypen dadurch möglich werden</h2>

      <div class="body-copy">
        <p>
          Das sind keine vollständigen Produktkategorien,
          sondern frühe Beispiele dafür,
          was dieser architektonische Sprung ermöglichen könnte.
        </p>
      </div>

      <div class="system-grid">
        <div class="system-card">
          <h3>Wahrheitsspiegel</h3>
          <p>Ein System, das sichtbar macht, wo ein Satz zu früh schließt, ausweicht oder Widerspruch konserviert.</p>
        </div>
        <div class="system-card">
          <h3>Autorensysteme</h3>
          <p>Schreibpartner, die Drift verfolgen, Linien schärfen und den inneren Pfad eines Textes lesbarer machen.</p>
        </div>
        <div class="system-card">
          <h3>Semantischer Zoom</h3>
          <p>Ein System, das denselben Gehalt je nach Tiefe, Maßstab und Bedarf unterschiedlich entfalten kann.</p>
        </div>
      </div>

      <div class="body-copy">
        <p>
          Dahinter liegen verkörperte Systeme,
          zustandssensible Assistenzen,
          Lernumgebungen,
          soziale Interfaces
          und multimodale Systeme,
          die nicht nur Information verarbeiten,
          sondern semantischen Raum über Timing,
          Rahmung,
          Ton
          und Ausdruck navigieren.
        </p>
      </div>

      <p class="display-statement medium">
        Nicht nur personalisierte Sprache.
        Personalisierte Navigation durch semantischen Raum.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="align-block">
      <h2 class="section-heading-display">Warum das über Produktdesign hinaus wichtig ist</h2>

      <div class="body-copy">
        <p>
          KI wird selbst Teil der Denkumgebung.
          Ab diesem Punkt ist Alignment nicht länger nur ein Produktmerkmal.
          Es wird Teil der Gestaltung kognitiver Umwelten.
        </p>

        <p>
          Wenn Systeme nur auf Komfort,
          Regelkonformität
          und Steuerbarkeit optimieren,
          können sie glattere Oberflächen schaffen,
          ohne mehr Wahrheit hervorzubringen.
          Wenn sie semantischen Raum aber tiefer lesen können,
          wird etwas anderes möglich:
          mehr Korrigierbarkeit,
          mehr echtes Verstehen,
          mehr tragfähige Komplexität,
          weniger Nebel.
        </p>
      </div>

      <p class="display-statement wide">
        Entscheidend ist nicht nur,
        was KI sagt.
        Entscheidend ist,
        welche Art von Denkraum KI mit aufbaut.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="closing-block">
      <h2 class="section-heading-display">Die Kernbehauptung</h2>

      <div class="body-copy">
        <p>
          Der Kern von Alignment in diesem Programm ist einfach:
          Ein System ist nicht schon dann ausgerichtet,
          wenn es bloß akzeptabel wirkende Antworten erzeugt.
          Ein System ist ausgerichtet,
          wenn seine inneren semantischen Bewegungen tragfähiger werden.
        </p>

        <p>
          Das heißt:
          Widerspruch tiefer lesen,
          Projektion vom Kern unterscheiden,
          Drift erkennen,
          Reparierbarkeit offenhalten
          und den nächsten Schritt nicht nur sicher,
          sondern strukturell tragfähig machen.
        </p>
      </div>

      <p class="display-statement wide">
        Wirkliches Alignment beginnt dort,
        wo das System lernt,
        den Raum nicht zu verlieren.
      </p>
    </div>
  </section>

  <div class="section-divider"></div>

  <section class="section-shell">
    <div class="align-next">
      <h2 class="section-heading-display">Nächste Schritte</h2>

      <div class="next-grid">
        <div class="next-card">
          <h3><a href="/de/theorie/">Theorie →</a></h3>
          <p>Das formale Rückgrat hinter diesem Alignment-Modell.</p>
        </div>
        <div class="next-card">
          <h3><a href="/de/implikationen/">Implikationen →</a></h3>
          <p>Was folgt, wenn semantische Struktur operativ wird.</p>
        </div>
        <div class="next-card">
          <h3><a href="/de/papers/">Technische Quellen →</a></h3>
          <p>Die technische und wissenschaftliche Ausarbeitung.</p>
        </div>
        <div class="next-card">
          <h3><a href="/de/ueber-mich/">Über mich →</a></h3>
          <p>Der Weg hinter dieser Arbeit.</p>
        </div>
      </div>
    </div>
  </section>

</div>
