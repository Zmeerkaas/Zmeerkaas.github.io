<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Spoti Guesser - Support</title>
  <meta name="description" content="Official support page for Spoti Guesser, a music-based game connected to Spotify." />

  <style>
    :root {
      --bg: #f7faf8;
      --surface: #ffffff;
      --text: #132018;
      --muted: #4a5a50;
      --line: #d9e5dd;
      --brand: #1db954;
      --brand-dark: #149143;
      --radius: 14px;
      --shadow: 0 8px 28px rgba(16, 32, 24, 0.08);
      --maxw: 1040px;
    }

    * { box-sizing: border-box; }

    html, body {
      margin: 0;
      padding: 0;
      font-family: "Segoe UI", "Helvetica Neue", Arial, sans-serif;
      color: var(--text);
      background:
        radial-gradient(1200px 500px at 20% -10%, #dff7e9 0%, rgba(223,247,233,0) 60%),
        radial-gradient(1000px 400px at 120% 10%, #eaf4ff 0%, rgba(234,244,255,0) 60%),
        var(--bg);
      line-height: 1.6;
      scroll-behavior: smooth;
    }

    a { color: var(--brand-dark); text-decoration: none; }
    a:hover { text-decoration: underline; }

    .container {
      width: min(var(--maxw), 92vw);
      margin: 0 auto;
    }

    header {
      position: sticky;
      top: 0;
      z-index: 100;
      backdrop-filter: blur(8px);
      background: rgba(247, 250, 248, 0.88);
      border-bottom: 1px solid var(--line);
    }

    .nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 16px;
      min-height: 68px;
    }

    .brand {
      font-size: 1.05rem;
      font-weight: 700;
    }

    .menu {
      list-style: none;
      display: flex;
      gap: 12px;
      margin: 0;
      padding: 0;
      flex-wrap: wrap;
    }

    .menu a {
      padding: 8px 12px;
      border-radius: 999px;
      font-weight: 600;
      font-size: 0.94rem;
      color: var(--text);
    }

    .menu a:hover {
      background: #fff;
      border: 1px solid var(--line);
    }

    .hero { padding: 60px 0 20px; }

    .hero-card {
      background: var(--surface);
      border: 1px solid var(--line);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      padding: 28px;
    }

    .kicker {
      background: #eaf8f0;
      color: #116437;
      padding: 4px 10px;
      border-radius: 999px;
      font-size: 0.75rem;
      font-weight: 700;
    }

    h1 { margin: 10px 0; }

    main { padding-bottom: 40px; }

    section {
      margin-top: 20px;
      background: var(--surface);
      border: 1px solid var(--line);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      padding: 22px;
    }

    .faq-list { display: grid; gap: 10px; }

    details {
      border: 1px solid var(--line);
      border-radius: 10px;
      padding: 10px;
      background: #fbfdfb;
    }

    summary { font-weight: 700; cursor: pointer; }

    .contact-box {
      padding: 12px;
      background: #f5fbf7;
      border: 1px solid #d6ecde;
      border-radius: 10px;
    }

    footer {
      margin-top: 30px;
      border-top: 1px solid var(--line);
      padding: 20px 0;
      font-size: 0.9rem;
      color: var(--muted);
    }

    .footer-inner {
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
    }
  </style>
</head>

<body>

<header>
  <nav class="container nav">
    <div class="brand">Spoti Guesser Support</div>
    <ul class="menu">
      <li><a href="#about">About</a></li>
      <li><a href="#support">Support</a></li>
      <li><a href="#faq">FAQ</a></li>
      <li><a href="#feedback">Feedback</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</header>

<div class="container hero">
  <div class="hero-card">
    <span class="kicker">Official Support</span>
    <h1>Help & Information</h1>
    <p>Welcome to the official support page for Spoti Guesser.</p>
  </div>
</div>

<main class="container">

<section id="about">
  <h2>About</h2>
  <p>Spoti Guesser is a music-based game connected to Spotify.</p>
</section>

<section id="support">
  <h2>Support</h2>
  <p>Check the FAQ below or try reconnecting Spotify.</p>
</section>

<section id="faq">
  <h2>FAQ</h2>
  <div class="faq-list">
    <details>
      <summary>Playback not working?</summary>
      <p>Reconnect Spotify and check internet.</p>
    </details>
  </div>
</section>

<section id="feedback">
  <h2>Feedback</h2>
  <p>Send us your ideas via email.</p>
</section>

<section id="contact">
  <h2>Contact</h2>
  <div class="contact-box">
    <strong>Email:</strong>
    <a href="mailto:support@yourapp.com">support@yourapp.com</a>
  </div>
</section>

</main>

<footer>
  <div class="container footer-inner">
    <span>Spoti Guesser</span>
    <span>&copy; 2026</span>
  </div>
</footer>

</body>
</html>
