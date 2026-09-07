<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Spoti Guesser — Support</title>
<meta name="description" content="Spoti Guesser is a music card game where you create and play your own Spotify-based party game." />

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;600;700&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">

<style>
  :root{
    --paper:#F1F7F0;
    --ink:#101E16;
    --muted:#52655A;
    --green:#1DB954;
    --green-dark:#148C3E;
    --coral:#FF5A5F;
    --tan:#EFE3C2;
    --line:#D8E3D9;
    --maxw:980px;
    --radius:10px;
  }

  *{box-sizing:border-box;}
  html{
    scroll-behavior:smooth;
    background:var(--paper);
  }

  html, body{
    width:100%;
    margin:0;
    overflow-x:hidden;
  }

  body{
    min-height:100vh;
    display:flex;
    flex-direction:column;
    background:var(--paper);
    color:var(--ink);
    font-family:'Inter', Arial, sans-serif;
    font-size:16px;
    line-height:1.55;
    -webkit-font-smoothing:antialiased;
  }

  main{
    flex:1 0 auto;
    width:100%;
  }

  header, footer, section{
    width:100%;
  }

  h1,h2,h3,.brand{
    font-family:'Space Grotesk', Arial, sans-serif;
    letter-spacing:-0.01em;
  }

  a{color:var(--green-dark);}
  a:focus-visible, button:focus-visible, summary:focus-visible{
    outline:2px solid var(--green-dark);
    outline-offset:3px;
  }

  .wrap{
    width:min(var(--maxw), 90vw);
    margin:0 auto;
  }

  /* ---------- header ---------- */
  header{
    position:sticky; top:0; z-index:10;
    background:rgba(241,247,240,0.92);
    backdrop-filter:blur(6px);
    border-bottom:1px solid var(--line);
  }
  .nav{
    display:flex;
    align-items:center;
    justify-content:space-between;
    padding:16px 0;
    gap:16px;
  }
  .brand{
    font-weight:700;
    font-size:1.15rem;
    color:var(--ink);
    display:flex;
    align-items:center;
    gap:8px;
    text-decoration:none;
  }
  .brand-dot{
    width:9px; height:9px; border-radius:50%;
    background:var(--green);
    display:inline-block;
  }
  .menu{
    display:flex;
    gap:22px;
    list-style:none;
    margin:0; padding:0;
    font-size:0.94rem;
  }
  .menu a{
    text-decoration:none;
    color:var(--ink);
    padding-bottom:3px;
    border-bottom:1px solid transparent;
    transition:border-color .15s ease;
  }
  .menu a:hover{ border-bottom-color:var(--green-dark); }

  /* ---------- hero ---------- */
  .hero{
    padding:64px 0 56px;
    display:grid;
    grid-template-columns:1.1fr 0.9fr;
    gap:48px;
    align-items:center;
  }
  .hero h1{
    font-size:clamp(2.2rem, 4.4vw, 3.4rem);
    line-height:1.05;
    margin:0 0 18px;
    font-weight:700;
  }
  .hero p{
    color:var(--muted);
    font-size:1.08rem;
    max-width:46ch;
    margin:0 0 26px;
  }
  .hero-actions{ display:flex; gap:12px; flex-wrap:wrap; }

  .btn{
    display:inline-block;
    font-family:'Inter', Arial, sans-serif;
    font-weight:600;
    font-size:0.95rem;
    padding:12px 20px;
    border-radius:999px;
    text-decoration:none;
    border:1px solid transparent;
  }
  .btn-primary{ background:var(--ink); color:var(--paper); }
  .btn-primary:hover{ background:var(--green-dark); }
  .btn-outline{ border-color:var(--ink); color:var(--ink); }
  .btn-outline:hover{ background:var(--ink); color:var(--paper); }

  /* the game card visual */
  .card-visual{
    position:relative;
    background:white;
    border:1.5px solid var(--ink);
    border-radius:16px;
    padding:22px;
    box-shadow:6px 6px 0 var(--green);
    max-width:320px;
    justify-self:end;
  }
  .card-visual .corner{
    position:absolute;
    width:9px; height:9px;
    border:1.5px solid var(--ink);
    border-radius:50%;
  }
  .corner.tl{ top:10px; left:10px; }
  .corner.tr{ top:10px; right:10px; }
  .corner.bl{ bottom:10px; left:10px; }
  .corner.br{ bottom:10px; right:10px; }
  .qr-grid{
    width:100%; aspect-ratio:1;
    margin:6px 0 16px;
    display:grid;
    grid-template-columns:repeat(7,1fr);
    grid-template-rows:repeat(7,1fr);
    gap:3px;
  }
  .qr-grid span{ background:var(--ink); border-radius:1px; }
  .qr-grid span.off{ background:transparent; }
  .card-visual .track{ font-weight:600; font-size:0.95rem; }
  .card-visual .meta{ color:var(--muted); font-size:0.85rem; margin-top:2px; }
  .card-visual hr{ border:none; border-top:1px dashed var(--line); margin:14px 0; }
  .card-visual .answer{ font-size:0.85rem; color:var(--muted); }
  .card-visual .answer b{ color:var(--ink); }

  /* ---------- sections ---------- */
  section{ padding:52px 0; border-top:1px solid var(--line); }
  section h2{
    font-size:1.6rem;
    margin:0 0 8px;
    font-weight:700;
  }
  .section-sub{ color:var(--muted); margin:0 0 28px; max-width:60ch; }

  .about-grid{
    display:grid;
    grid-template-columns:1.3fr 0.7fr;
    gap:44px;
    align-items:start;
  }
  .about-grid p{ margin:0 0 16px; color:var(--ink); }
  .about-grid p:last-of-type{ margin-bottom:0; }

  .credit{
    background:var(--tan);
    border-radius:var(--radius);
    padding:18px 20px;
    font-size:0.92rem;
  }
  .credit .who{ font-weight:600; margin-top:6px; }

  /* download */
  .download-actions{ display:flex; gap:12px; flex-wrap:wrap; }

  /* how it works — a genuine sequence, numbered */
  .steps{
    list-style:none;
    margin:0; padding:0;
    counter-reset:step;
    display:grid;
    gap:0;
  }
  .steps li{
    counter-increment:step;
    display:flex;
    gap:18px;
    padding:16px 0;
    border-bottom:1px solid var(--line);
  }
  .steps li:last-child{ border-bottom:none; }
  .steps li::before{
    content: counter(step);
    font-family:'Space Grotesk', Arial, sans-serif;
    font-weight:600;
    font-size:1rem;
    color:var(--green-dark);
    border:1.5px solid var(--green-dark);
    border-radius:50%;
    width:30px; height:30px;
    flex:none;
    display:flex; align-items:center; justify-content:center;
  }
  .steps li span{ padding-top:4px; }

  /* support callout */
  .support-card{
    display:flex;
    align-items:flex-start;
    gap:18px;
    background:var(--tan);
    border-left:4px solid var(--green-dark);
    border-radius:var(--radius);
    padding:22px 24px;
  }
  .support-card .glyph{
    flex:none;
    width:38px; height:38px;
    border-radius:50%;
    background:var(--ink);
    color:var(--paper);
    font-family:'Space Grotesk', Arial, sans-serif;
    font-weight:600;
    display:flex; align-items:center; justify-content:center;
    font-size:1.1rem;
  }
  .support-card p{ margin:0; color:var(--ink); }
  .support-card p + p{ margin-top:6px; }

  /* faq */
  .faq-list{ border-top:1px solid var(--line); }
  .faq-list details{
    border-bottom:1px solid var(--line);
    padding:16px 0;
  }
  .faq-list summary{
    cursor:pointer;
    font-weight:600;
    list-style:none;
    display:flex;
    justify-content:space-between;
    align-items:center;
    gap:12px;
  }
  .faq-list summary::-webkit-details-marker{ display:none; }
  .faq-list summary::after{
    content:"+";
    font-family:'Space Grotesk', Arial, sans-serif;
    font-size:1.2rem;
    color:var(--green-dark);
    flex:none;
  }
  .faq-list details[open] summary::after{ content:"−"; }
  .faq-list p{ color:var(--muted); margin:10px 0 0; max-width:65ch; }

  /* closing band: support / donate / contact */
  .closing{
    background:var(--ink);
    color:var(--paper);
    border-top:none;
  }
  .closing h2{ color:var(--paper); }
  .closing .section-sub{ color:#B9C8BE; }
  .closing-grid{
    display:grid;
    grid-template-columns:repeat(3, 1fr);
    gap:32px;
  }
  .closing-col p{ color:#CFDDD3; margin:0 0 14px; font-size:0.95rem; }
  .closing a.inline{ color:var(--green); }
  .closing .btn-donate{
    background:var(--green);
    color:var(--ink);
  }
  .closing .btn-donate:hover{ background:#22e267; }
  .closing-col h3{
    font-size:1rem;
    margin:0 0 10px;
    font-weight:600;
  }

  footer{
    text-align:center;
    padding:22px 0;
    color:var(--muted);
    font-size:0.85rem;
  }

  @media (max-width:760px){
    .nav{ flex-direction:column; align-items:flex-start; gap:10px; }
    .menu{ flex-wrap:wrap; gap:10px 16px; }
    .hero{ grid-template-columns:1fr; padding-top:40px; }
    .card-visual{ justify-self:start; max-width:280px; }
    .about-grid{ grid-template-columns:1fr; }
    .closing-grid{ grid-template-columns:1fr; gap:26px; }
  }

  @media (prefers-reduced-motion: reduce){
    html{ scroll-behavior:auto; }
    *{ transition:none !important; }
  }
</style>
</head>

<body>

<header>
  <nav class="wrap nav">
    <a class="brand" href="#top"><span class="brand-dot"></span>Spoti Guesser</a>
    <ul class="menu">
      <li><a href="#about">About</a></li>
      <li><a href="#how">How it works</a></li>
      <li><a href="#faq">FAQ</a></li>
      <li><a href="#donate">Support us</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</header>

<main>

  <div class="wrap hero" id="top">
    <div>
      <h1>Turn your living room into a music quiz arena.</h1>
      <p>Spoti Guesser is a card game you build from your own Spotify playlists. Generate QR cards, print them, scan during play, and guess the title, artist and year before your friends do.</p>
      <div class="hero-actions">
        <a class="btn btn-primary" href="https://play.google.com/store/apps/details?id=com.spotiguesser.app" target="_blank" rel="noopener noreferrer">Download for Android</a>
        <a class="btn btn-outline" href="https://apps.apple.com/us/app/spoti-guesser/id6760561686" target="_blank" rel="noopener noreferrer">Download for iOS</a>
      </div>
    </div>

    <div class="card-visual" aria-hidden="true">
      <span class="corner tl"></span><span class="corner tr"></span><span class="corner bl"></span><span class="corner br"></span>
      <div class="qr-grid">
        <!-- decorative qr-like pattern -->
        <span></span><span></span><span class="off"></span><span></span><span class="off"></span><span></span><span></span>
        <span></span><span class="off"></span><span></span><span></span><span></span><span class="off"></span><span></span>
        <span></span><span></span><span class="off"></span><span class="off"></span><span class="off"></span><span></span><span></span>
        <span class="off"></span><span></span><span></span><span class="off"></span><span></span><span></span><span class="off"></span>
        <span></span><span></span><span class="off"></span><span class="off"></span><span class="off"></span><span></span><span></span>
        <span></span><span class="off"></span><span></span><span></span><span></span><span class="off"></span><span></span>
        <span></span><span></span><span class="off"></span><span></span><span class="off"></span><span></span><span></span>
      </div>
      <div class="track">Track #014</div>
      <div class="meta">Scan to play this round</div>
      <hr />
      <div class="answer">Title, artist & year on the <b>back of the card</b></div>
    </div>
  </div>

  <section id="about">
    <div class="wrap about-grid">
      <div>
        <h2>About the app</h2>
        <p class="section-sub" style="margin-top:-4px;">A social music game built for discovery, memory and friendly rivalry.</p>
        <p>Spoti Guesser turns Spotify music into playable QR cards. Scan a card, start the track, and let everyone guess the song title, artist and release year. It combines the energy of a party game with the personal touch of your own playlists, so every round feels unique to your group.</p>
        <p>Use it as a quick casual game in the living room, a competitive challenge at parties, or a custom trivia format for birthdays and events. Connect Spotify to unlock direct playback and support for more playlist types, or skip it entirely and play in guest mode — the core game works either way.</p>
        <p>The full loop: generate cards from a playlist, album or track, export and print them, scan during gameplay, and verify answers with the card back. Build a set once and keep reusing it, so the game feels like a real tabletop title with the convenience of a mobile app.</p>
      </div>
      <div class="credit">
        <p style="margin:0;">Spoti Guesser is a passion project built by two students who wanted to bring people together through music, competition and shared memories.</p>
        <div class="who">Joris — development<br />Tim — design</div>
      </div>
    </div>
  </section>

  <section id="download">
    <div class="wrap">
      <h2>Download now</h2>
      <p class="section-sub">Start creating your own QR music cards in minutes.</p>
      <div class="download-actions">
        <a class="btn btn-primary" href="https://play.google.com/store/apps/details?id=com.spotiguesser.app" target="_blank" rel="noopener noreferrer">Download for Android</a>
        <a class="btn btn-outline" href="https://apps.apple.com/us/app/spoti-guesser/id6760561686" target="_blank" rel="noopener noreferrer">Download for iOS</a>
      </div>
    </div>
  </section>

  <section id="how">
    <div class="wrap">
      <h2>How it works</h2>
      <p class="section-sub">Four steps from playlist to party.</p>
      <ol class="steps">
        <li><span>Generate QR cards from a Spotify playlist, album or track.</span></li>
        <li><span>Print them and write the song info on the back.</span></li>
        <li><span>Scan a card during the game to start playback.</span></li>
        <li><span>Guess the song, artist or year before anyone else.</span></li>
      </ol>
    </div>
  </section>

  <section id="faq">
    <div class="wrap">
      <h2>FAQ</h2>
      <p class="section-sub">Everything about setup, playing and printing.</p>
      <div class="faq-list">
        <details>
          <summary>What is Spoti Guesser?</summary>
          <p>A music card game app where you scan QR cards and players guess the artist, title and year.</p>
        </details>
        <details>
          <summary>Do I need Spotify?</summary>
          <p>No, Spotify is optional. However, for features like direct playback and some playlists, Spotify is required.</p>
        </details>
        <details>
          <summary>Can I play without Spotify?</summary>
          <p>Yes, you can play in guest mode. Some advanced features will be limited.</p>
        </details>
        <details>
          <summary>How do I start a game?</summary>
          <p>Tap Start Game, scan a card, and let players guess. Use the back of the card to verify answers.</p>
        </details>
        <details>
          <summary>How do I create QR cards?</summary>
          <p>Go to Generate QR Codes, paste a Spotify link (playlist, album or track), and export your cards as a PDF.</p>
        </details>
        <details>
          <summary>Which Spotify links are supported?</summary>
          <p>Links to playlists, albums and individual tracks are supported.</p>
        </details>
        <details>
          <summary>Can I use private playlists?</summary>
          <p>Yes, but only if you're logged into Spotify and have access to that private playlist.</p>
        </details>
        <details>
          <summary>Why does the app request camera access?</summary>
          <p>The camera is required to scan QR codes on the game cards.</p>
        </details>
        <details>
          <summary>The QR code doesn't scan, what should I do?</summary>
          <p>Make sure there's enough light, hold your camera steady, and check that the print is sharp and not damaged.</p>
        </details>
        <details>
          <summary>Playback isn't working, what can I do?</summary>
          <p>Check your internet connection, log back into Spotify, and try scanning again.</p>
        </details>
        <details>
          <summary>Can I print cards?</summary>
          <p>Yes, you can export cards and print them on paper or cardstock for physical game nights.</p>
        </details>
        <details>
          <summary>Why do colors sometimes look different when printed?</summary>
          <p>Colors may vary due to screen settings, printer profiles, paper and ink. Always test with a sample print first.</p>
        </details>
        <details>
          <summary>Which languages does the app support?</summary>
          <p>The app supports multiple languages, including Dutch and English.</p>
        </details>
        <details>
          <summary>What about privacy?</summary>
          <p>Privacy information can be found in the app under Privacy Policy in the settings.</p>
        </details>
        <details>
          <summary>How do I contact support?</summary>
          <p>For questions, feedback or bugs, you can email BWBBstudio@gmail.com.</p>
        </details>
      </div>
    </div>
  </section>

  <section id="support">
    <div class="wrap">
      <h2>Need help?</h2>
      <p class="section-sub">A few quick fixes before you reach out.</p>
      <div class="support-card">
        <span class="glyph" aria-hidden="true">?</span>
        <div>
          <p>Having issues? Try reconnecting Spotify, updating the app, or restarting your device.</p>
          <p>Still stuck? Reach out via the contact details below and we'll help you out.</p>
        </div>
      </div>
    </div>
  </section>

  <section class="closing" id="donate">
    <div class="wrap">
      <h2>Support us, get in touch</h2>
      <p class="section-sub">Spoti Guesser is a student project, kept alive by players like you.</p>
      <div class="closing-grid">
        <div class="closing-col">
          <h3>Support the project</h3>
          <p>If you enjoy the game, consider chipping in to help cover development costs.</p>
          <a class="btn btn-donate" href="https://www.paypal.com/paypalme/JSmeerkaas" target="_blank" rel="noopener noreferrer">Donate via PayPal</a>
        </div>
        <div class="closing-col" id="contact">
          <h3>Contact</h3>
          <p>Questions, feedback or bugs — we usually reply within 24–48 hours.</p>
          <a class="inline" href="mailto:BWBBstudio@gmail.com">BWBBstudio@gmail.com</a>
        </div>
        <div class="closing-col">
          <h3>Made by</h3>
          <p>Joris (development) &amp; Tim (design) — two students building for music lovers.</p>
        </div>
      </div>
    </div>
  </section>

</main>

<footer>
  <p>© 2026 Spoti Guesser</p>
</footer>

</body>
</html>
