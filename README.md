<!DOCTYPE html>
<html lang="it">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Privacy Policy — Palestra No Limits</title>
  <link href="https://fonts.googleapis.com/css2?family=DM+Sans:ital,wght@0,300;0,400;0,500;0,700;1,300&family=DM+Serif+Display&display=swap" rel="stylesheet" />
  <style>
    :root {
      --red:    #ff0000;
      --blue:   #0004AD;
      --yellow: #ffef00;
      --black:  #212121;
      --white:  #ffffff;
      --gray:   #f4f4f4;
      --muted:  #6b6b6b;
      --border: #e0e0e0;
    }

    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    html { scroll-behavior: smooth; }

    body {
      font-family: 'DM Sans', sans-serif;
      background: var(--white);
      color: var(--black);
      font-size: 16px;
      line-height: 1.75;
    }

    /* ── HEADER ── */
    header {
      background: var(--black);
      color: var(--white);
      padding: 0;
      position: sticky;
      top: 0;
      z-index: 100;
      border-bottom: 3px solid var(--red);
    }
    .header-inner {
      max-width: 860px;
      margin: 0 auto;
      padding: 18px 24px;
      display: flex;
      align-items: center;
      gap: 16px;
    }
    .logo-mark {
      width: 38px;
      height: 38px;
      background: var(--red);
      border-radius: 6px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-family: 'DM Serif Display', serif;
      font-size: 20px;
      color: var(--white);
      letter-spacing: -1px;
      flex-shrink: 0;
    }
    .header-text h1 {
      font-size: 15px;
      font-weight: 700;
      letter-spacing: 0.04em;
      text-transform: uppercase;
      color: var(--white);
      line-height: 1.2;
    }
    .header-text span {
      font-size: 12px;
      color: rgba(255,255,255,0.5);
      font-weight: 300;
      letter-spacing: 0.02em;
    }

    /* ── HERO BAND ── */
    .hero-band {
      background: var(--gray);
      border-bottom: 1px solid var(--border);
    }
    .hero-inner {
      max-width: 860px;
      margin: 0 auto;
      padding: 48px 24px 40px;
    }
    .pill {
      display: inline-block;
      background: var(--red);
      color: var(--white);
      font-size: 11px;
      font-weight: 700;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      padding: 4px 12px;
      border-radius: 100px;
      margin-bottom: 16px;
    }
    .hero-inner h2 {
      font-family: 'DM Serif Display', serif;
      font-size: clamp(28px, 5vw, 40px);
      line-height: 1.15;
      color: var(--black);
      max-width: 600px;
    }
    .hero-inner h2 em {
      font-style: normal;
      color: var(--blue);
    }
    .meta {
      margin-top: 20px;
      display: flex;
      gap: 24px;
      flex-wrap: wrap;
    }
    .meta-item {
      font-size: 13px;
      color: var(--muted);
    }
    .meta-item strong { color: var(--black); }

    /* ── TOC ── */
    .toc-wrapper {
      max-width: 860px;
      margin: 0 auto;
      padding: 32px 24px 0;
    }
    .toc {
      background: var(--white);
      border: 1px solid var(--border);
      border-left: 4px solid var(--blue);
      border-radius: 8px;
      padding: 20px 24px;
    }
    .toc h3 {
      font-size: 12px;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      color: var(--blue);
      margin-bottom: 12px;
    }
    .toc ol {
      padding-left: 18px;
    }
    .toc ol li {
      font-size: 14px;
      margin-bottom: 4px;
    }
    .toc ol li a {
      color: var(--black);
      text-decoration: none;
      transition: color 0.2s;
    }
    .toc ol li a:hover { color: var(--red); }

    /* ── MAIN CONTENT ── */
    main {
      max-width: 860px;
      margin: 0 auto;
      padding: 40px 24px 80px;
    }

    section {
      margin-bottom: 52px;
      scroll-margin-top: 80px;
    }

    .section-number {
      font-size: 11px;
      font-weight: 700;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: var(--red);
      margin-bottom: 6px;
    }

    section h2 {
      font-family: 'DM Serif Display', serif;
      font-size: 22px;
      color: var(--black);
      margin-bottom: 16px;
      padding-bottom: 12px;
      border-bottom: 1px solid var(--border);
    }

    section p {
      font-size: 15.5px;
      color: #333;
      margin-bottom: 12px;
    }

    section ul, section ol {
      padding-left: 20px;
      margin-bottom: 12px;
    }
    section ul li, section ol li {
      font-size: 15.5px;
      color: #333;
      margin-bottom: 6px;
    }

    /* Info box */
    .info-box {
      background: #f0f4ff;
      border-left: 4px solid var(--blue);
      border-radius: 0 8px 8px 0;
      padding: 16px 20px;
      margin: 20px 0;
    }
    .info-box p {
      font-size: 14px;
      color: var(--blue);
      margin: 0;
    }
    .info-box strong { color: var(--black); }

    /* Warning box */
    .warn-box {
      background: #fff5f5;
      border-left: 4px solid var(--red);
      border-radius: 0 8px 8px 0;
      padding: 16px 20px;
      margin: 20px 0;
    }
    .warn-box p {
      font-size: 14px;
      color: #cc0000;
      margin: 0;
    }

    /* Table */
    .table-wrap { overflow-x: auto; margin: 20px 0; }
    table {
      width: 100%;
      border-collapse: collapse;
      font-size: 14px;
    }
    thead tr { background: var(--black); color: var(--white); }
    thead th {
      padding: 12px 16px;
      text-align: left;
      font-weight: 600;
      font-size: 12px;
      letter-spacing: 0.05em;
      text-transform: uppercase;
    }
    tbody tr { border-bottom: 1px solid var(--border); }
    tbody tr:last-child { border-bottom: none; }
    tbody td { padding: 12px 16px; color: #444; vertical-align: top; }
    tbody tr:nth-child(even) { background: var(--gray); }

    /* Contact card */
    .contact-card {
      background: var(--black);
      color: var(--white);
      border-radius: 12px;
      padding: 28px 28px;
      margin-top: 20px;
    }
    .contact-card h3 {
      font-family: 'DM Serif Display', serif;
      font-size: 18px;
      margin-bottom: 16px;
      color: var(--white);
    }
    .contact-row {
      display: flex;
      gap: 8px;
      align-items: flex-start;
      margin-bottom: 10px;
      font-size: 14.5px;
      color: rgba(255,255,255,0.8);
    }
    .contact-label {
      font-size: 11px;
      font-weight: 700;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--red);
      min-width: 120px;
      padding-top: 1px;
    }

    /* ── FOOTER ── */
    footer {
      background: var(--gray);
      border-top: 1px solid var(--border);
      padding: 28px 24px;
      text-align: center;
    }
    footer p {
      font-size: 13px;
      color: var(--muted);
    }
    footer p strong { color: var(--black); }

    @media (max-width: 600px) {
      .meta { flex-direction: column; gap: 8px; }
      .contact-row { flex-direction: column; gap: 2px; }
      .contact-label { min-width: unset; }
    }
  </style>
</head>
<body>

<!-- HEADER -->
<header>
  <div class="header-inner">
    <div class="logo-mark">NL</div>
    <div class="header-text">
      <h1>Palestra No Limits</h1>
      <span>Informativa sulla Privacy — Art. 13 GDPR</span>
    </div>
  </div>
</header>

<!-- HERO BAND -->
<div class="hero-band">
  <div class="hero-inner">
    <span class="pill">Documento Legale</span>
    <h2>Informativa sul trattamento dei <em>dati personali</em></h2>
    <div class="meta">
      <div class="meta-item"><strong>Versione:</strong> 1.0</div>
      <div class="meta-item"><strong>Data di entrata in vigore:</strong> <span id="current-date"></span></div>
      <div class="meta-item"><strong>Normativa:</strong> Reg. UE 2016/679 (GDPR) — D.Lgs. 196/2003</div>
    </div>
  </div>
</div>

<!-- TABLE OF CONTENTS -->
<div class="toc-wrapper">
  <div class="toc">
    <h3>Indice</h3>
    <ol>
      <li><a href="#s1">Titolare del Trattamento</a></li>
      <li><a href="#s2">Tipologia di Dati Raccolti</a></li>
      <li><a href="#s3">Finalità e Basi Giuridiche del Trattamento</a></li>
      <li><a href="#s4">Modalità del Trattamento</a></li>
      <li><a href="#s5">Condivisione con Terze Parti (Meta Platforms)</a></li>
      <li><a href="#s6">Conservazione dei Dati</a></li>
      <li><a href="#s7">Trasferimento dei Dati Extra-UE</a></li>
      <li><a href="#s8">Diritti dell'Interessato</a></li>
      <li><a href="#s9">Cookie e Tecnologie di Tracciamento</a></li>
      <li><a href="#s10">Modifiche alla Privacy Policy</a></li>
      <li><a href="#s11">Contatti e Reclami</a></li>
    </ol>
  </div>
</div>

<!-- MAIN CONTENT -->
<main>

  <!-- 1 -->
  <section id="s1">
    <div class="section-number">Articolo 01</div>
    <h2>Titolare del Trattamento</h2>
    <p>
      Il Titolare del trattamento dei dati personali, ai sensi dell'art. 4 n. 7 del Regolamento UE 2016/679 (di seguito "GDPR"), è:
    </p>
    <div class="contact-card">
      <h3>Dati del Titolare</h3>
      <div class="contact-row">
        <span class="contact-label">Ragione sociale</span>
        <span>Palestra No Limits</span>
      </div>
      <div class="contact-row">
        <span class="contact-label">Indirizzo</span>
        <span>Via Kennedy 310, 98051 Barcellona Pozzo di Gotto (ME), Italia</span>
      </div>
      <div class="contact-row">
        <span class="contact-label">Profilo Instagram</span>
        <span>@gymnolimits_ff</span>
      </div>
      <div class="contact-row">
        <span class="contact-label">Email di contatto</span>
        <span>gymnolimitsff@gmail.com</span>
      </div>
    </div>
  </section>

  <!-- 2 -->
  <section id="s2">
    <div class="section-number">Articolo 02</div>
    <h2>Tipologia di Dati Raccolti</h2>
    <p>
      Nell'ambito delle attività promozionali condotte tramite le piattaforme Meta (Facebook e Instagram), il Titolare raccoglie le seguenti categorie di dati personali:
    </p>
    <div class="table-wrap">
      <table>
        <thead>
          <tr>
            <th>Categoria</th>
            <th>Tipologia di dato</th>
            <th>Fonte</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td><strong>Dati anagrafici</strong></td>
            <td>Nome e cognome</td>
            <td>Compilazione modulo lead / form Meta</td>
          </tr>
          <tr>
            <td><strong>Dati di contatto</strong></td>
            <td>Numero di telefono, indirizzo email</td>
            <td>Compilazione modulo lead / form Meta</td>
          </tr>
          <tr>
            <td><strong>Dati di navigazione</strong></td>
            <td>Indirizzo IP, dati cookie, interazioni con le inserzioni</td>
            <td>Meta Pixel / tecnologie di tracciamento Meta</td>
          </tr>
          <tr>
            <td><strong>Dati comportamentali</strong></td>
            <td>Visualizzazioni, click, interazioni con i contenuti pubblicati</td>
            <td>Piattaforme Meta (Facebook/Instagram)</td>
          </tr>
        </tbody>
      </table>
    </div>
    <div class="warn-box">
      <p>Non vengono raccolte categorie particolari di dati ai sensi dell'art. 9 GDPR (dati sanitari, biometrici, religiosi, politici, ecc.).</p>
    </div>
  </section>

  <!-- 3 -->
  <section id="s3">
    <div class="section-number">Articolo 03</div>
    <h2>Finalità e Basi Giuridiche del Trattamento</h2>
    <p>I dati raccolti sono trattati per le seguenti finalità, ciascuna fondata sulla relativa base giuridica ai sensi dell'art. 6 GDPR:</p>
    <div class="table-wrap">
      <table>
        <thead>
          <tr>
            <th>Finalità</th>
            <th>Base giuridica</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td><strong>Risposta a richieste di informazioni</strong> su iscrizioni, promozioni e corsi</td>
            <td>Art. 6(1)(b) GDPR — Esecuzione di misure precontrattuali</td>
          </tr>
          <tr>
            <td><strong>Invio di comunicazioni commerciali</strong> e promozioni (via telefono, WhatsApp, email)</td>
            <td>Art. 6(1)(a) GDPR — Consenso esplicito dell'interessato</td>
          </tr>
          <tr>
            <td><strong>Attività di marketing tramite Meta Ads</strong> (inserzioni personalizzate, pubblici simili)</td>
            <td>Art. 6(1)(a) GDPR — Consenso esplicito dell'interessato</td>
          </tr>
          <tr>
            <td><strong>Analisi delle prestazioni delle campagne pubblicitarie</strong> (report, ottimizzazione)</td>
            <td>Art. 6(1)(f) GDPR — Legittimo interesse del Titolare</td>
          </tr>
          <tr>
            <td><strong>Adempimento di obblighi di legge</strong> (fiscali, contabili, amministrativi)</td>
            <td>Art. 6(1)(c) GDPR — Obbligo legale</td>
          </tr>
        </tbody>
      </table>
    </div>
    <div class="info-box">
      <p><strong>Nota sul consenso:</strong> Dove il trattamento è basato sul consenso (art. 6(1)(a)), l'interessato ha il diritto di revocarlo in qualsiasi momento senza pregiudicare la liceità del trattamento effettuato prima della revoca.</p>
    </div>
  </section>

  <!-- 4 -->
  <section id="s4">
    <div class="section-number">Articolo 04</div>
    <h2>Modalità del Trattamento</h2>
    <p>
      Il trattamento dei dati personali viene effettuato con strumenti elettronici e/o cartacei, nel rispetto dei principi di liceità, correttezza, trasparenza, minimizzazione e integrità previsti dall'art. 5 GDPR.
    </p>
    <p>I dati sono trattati da:</p>
    <ul>
      <li>Il Titolare del trattamento e il personale da esso autorizzato;</li>
      <li>Eventuali collaboratori esterni o consulenti di marketing (es. Social Media Manager), vincolati da specifici accordi di riservatezza e designati come Responsabili del trattamento ex art. 28 GDPR.</li>
    </ul>
  </section>

  <!-- 5 -->
  <section id="s5">
    <div class="section-number">Articolo 05</div>
    <h2>Condivisione con Terze Parti — Meta Platforms</h2>
    <p>
      Il Titolare utilizza i servizi pubblicitari di <strong>Meta Platforms Ireland Ltd.</strong> (Facebook e Instagram) per la diffusione di inserzioni promozionali. In questo contesto:
    </p>
    <ul>
      <li>Meta agisce come <strong>titolare autonomo</strong> del trattamento per i propri servizi di piattaforma;</li>
      <li>I dati raccolti attraverso i moduli lead di Meta (Lead Ads) sono trasmessi al Titolare nel rispetto delle condizioni d'uso di Meta;</li>
      <li>Meta può utilizzare i dati degli utenti che interagiscono con le inserzioni per finalità proprie, secondo la propria <a href="https://www.facebook.com/privacy/policy/" target="_blank" rel="noopener">Informativa sulla Privacy</a>.</li>
    </ul>
    <div class="info-box">
      <p>Puoi gestire le tue preferenze pubblicitarie su Meta visitando: <strong>Impostazioni Facebook → Inserzioni → Preferenze inserzioni</strong>.</p>
    </div>
    <p>
      Il Titolare non cede, vende o trasferisce i dati personali a terze parti per finalità proprie di questi ultimi, salvo espressa indicazione contraria e raccolta del consenso.
    </p>
  </section>

  <!-- 6 -->
  <section id="s6">
    <div class="section-number">Articolo 06</div>
    <h2>Conservazione dei Dati</h2>
    <p>I dati sono conservati per il tempo strettamente necessario alle finalità per le quali sono stati raccolti:</p>
    <div class="table-wrap">
      <table>
        <thead>
          <tr>
            <th>Finalità</th>
            <th>Periodo di conservazione</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Risposta a richieste di contatto / preventivi</td>
            <td>12 mesi dalla richiesta, salvo instaurazione di un rapporto contrattuale</td>
          </tr>
          <tr>
            <td>Gestione del rapporto contrattuale (iscrizione)</td>
            <td>Durata del contratto + 10 anni per obblighi fiscali (art. 2220 c.c.)</td>
          </tr>
          <tr>
            <td>Marketing e comunicazioni commerciali</td>
            <td>Fino alla revoca del consenso o, in assenza di attività, 24 mesi</td>
          </tr>
          <tr>
            <td>Dati di navigazione e cookie pubblicitari</td>
            <td>Secondo le politiche di Meta (in genere 90–180 giorni)</td>
          </tr>
        </tbody>
      </table>
    </div>
    <p>Alla scadenza del termine, i dati saranno cancellati o resi anonimi in modo irreversibile.</p>
  </section>

  <!-- 7 -->
  <section id="s7">
    <div class="section-number">Articolo 07</div>
    <h2>Trasferimento dei Dati Extra-UE</h2>
    <p>
      I dati trattati tramite Meta Platforms potrebbero essere trasferiti negli <strong>Stati Uniti d'America</strong> o in altri Paesi extra-UE. Tale trasferimento avviene nel rispetto delle garanzie previste dagli artt. 44–49 GDPR, in particolare sulla base di:
    </p>
    <ul>
      <li>Clausole contrattuali standard approvate dalla Commissione Europea;</li>
      <li>Adeguate misure di sicurezza implementate da Meta Platforms (certificazione Data Privacy Framework UE-USA, ove applicabile).</li>
    </ul>
  </section>

  <!-- 8 -->
  <section id="s8">
    <div class="section-number">Articolo 08</div>
    <h2>Diritti dell'Interessato</h2>
    <p>Ai sensi degli artt. 15–22 GDPR, l'interessato ha il diritto di:</p>
    <ul>
      <li><strong>Accesso</strong> (art. 15) — ottenere conferma del trattamento e copia dei propri dati;</li>
      <li><strong>Rettifica</strong> (art. 16) — correggere dati inesatti o incompleti;</li>
      <li><strong>Cancellazione</strong> (art. 17) — ottenere la rimozione dei propri dati ("diritto all'oblio");</li>
      <li><strong>Limitazione</strong> (art. 18) — limitare il trattamento in determinati casi;</li>
      <li><strong>Portabilità</strong> (art. 20) — ricevere i propri dati in formato strutturato e leggibile da macchina;</li>
      <li><strong>Opposizione</strong> (art. 21) — opporsi al trattamento per finalità di marketing diretto;</li>
      <li><strong>Revoca del consenso</strong> — in qualsiasi momento, senza effetti retroattivi.</li>
    </ul>
    <p>
      Per esercitare tali diritti, l'interessato può contattare il Titolare all'indirizzo email indicato nella sezione 1.
      Il Titolare risponderà entro <strong>30 giorni</strong> dalla ricezione della richiesta (art. 12 GDPR), con possibilità di proroga di ulteriori 60 giorni in casi di complessità.
    </p>
  </section>

  <!-- 9 -->
  <section id="s9">
    <div class="section-number">Articolo 09</div>
    <h2>Cookie e Tecnologie di Tracciamento</h2>
    <p>
      Il Titolare utilizza il <strong>Meta Pixel</strong> (ora "Meta Business Tools") sulle proprie pagine e campagne promozionali. Si tratta di un frammento di codice che consente a Meta di:
    </p>
    <ul>
      <li>Misurare l'efficacia delle inserzioni pubblicitarie;</li>
      <li>Ottimizzare la distribuzione degli annunci;</li>
      <li>Creare pubblici personalizzati e simili (<em>Custom Audiences</em>, <em>Lookalike Audiences</em>).</li>
    </ul>
    <p>
      L'utilizzo del Meta Pixel è soggetto al consenso dell'utente secondo le proprie impostazioni sulla piattaforma Meta. Per maggiori informazioni: <a href="https://www.facebook.com/business/help/742478679120153" target="_blank" rel="noopener">Meta Pixel — Informazioni</a>.
    </p>
  </section>

  <!-- 10 -->
  <section id="s10">
    <div class="section-number">Articolo 10</div>
    <h2>Modifiche alla Privacy Policy</h2>
    <p>
      Il Titolare si riserva il diritto di modificare la presente informativa in qualsiasi momento, in particolare a seguito di aggiornamenti normativi, giurisprudenziali o tecnologici.
    </p>
    <p>
      Le modifiche saranno pubblicate su questa pagina con aggiornamento della data di entrata in vigore. In caso di modifiche sostanziali, l'interessato verrà informato attraverso i canali di comunicazione disponibili.
    </p>
    <p>
      Si invita l'utente a consultare periodicamente questa pagina.
    </p>
  </section>

  <!-- 11 -->
  <section id="s11">
    <div class="section-number">Articolo 11</div>
    <h2>Contatti e Reclami</h2>
    <p>Per qualsiasi richiesta relativa al trattamento dei propri dati personali, è possibile contattare il Titolare ai recapiti indicati nella sezione 1.</p>
    <p>
      L'interessato ha inoltre il diritto di proporre reclamo all'autorità di controllo competente. In Italia, tale autorità è il:
    </p>
    <div class="contact-card">
      <h3>Garante per la Protezione dei Dati Personali</h3>
      <div class="contact-row">
        <span class="contact-label">Sito web</span>
        <span><a href="https://www.garanteprivacy.it" target="_blank" rel="noopener" style="color:var(--yellow);">www.garanteprivacy.it</a></span>
      </div>
      <div class="contact-row">
        <span class="contact-label">Indirizzo</span>
        <span>Piazza Venezia 11, 00187 Roma</span>
      </div>
      <div class="contact-row">
        <span class="contact-label">Email</span>
        <span>garante@gpdp.it</span>
      </div>
      <div class="contact-row">
        <span class="contact-label">PEC</span>
        <span>protocollo@pec.gpdp.it</span>
      </div>
    </div>
  </section>

</main>

<!-- FOOTER -->
<footer>
  <p><strong>Palestra No Limits</strong> — Via Kennedy 310, Barcellona P.G. (ME)</p>
  <p style="margin-top:6px;">Informativa redatta ai sensi dell'art. 13 del Regolamento UE 2016/679 (GDPR) e del D.Lgs. 196/2003 come modificato dal D.Lgs. 101/2018.</p>
  <p style="margin-top:6px; font-size:12px; color:#999;">© <span id="year"></span> Palestra No Limits. Tutti i diritti riservati.</p>
</footer>

<script>
  // Dynamic date
  const d = new Date();
  const months = ['Gennaio','Febbraio','Marzo','Aprile','Maggio','Giugno','Luglio','Agosto','Settembre','Ottobre','Novembre','Dicembre'];
  document.getElementById('current-date').textContent = d.getDate() + ' ' + months[d.getMonth()] + ' ' + d.getFullYear();
  document.getElementById('year').textContent = d.getFullYear();
</script>
</body>
</html>
