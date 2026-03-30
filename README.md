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

    a {
      color: var(--brand-dark);
      text-decoration: none;
      transition: opacity 0.2s ease;
    }

    a:hover {
      text-decoration: underline;
      opacity: 0.8;
    }

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
      padding: 0 12px;
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
      border: 1px solid transparent;
    }

    .menu a:hover {
      background: #fff;
      border: 1px solid var(--line);
    }

    .hero {
      padding: 64px 0 28px;
    }

    .hero-card {
      background: var(--surface);
      border: 1px solid var(--line);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      padding: 30px;
    }

    .kicker {
      display: inline-block;
      background: #eaf8f0;
      color: #116437;
      border: 1px solid #c9ebd7;
      padding: 4px 10px;
      border-radius: 999px;
      font-size: 0.78rem;
      font-weight: 700;
      text-transform: uppercase;
    }

    main { padding-bottom: 40px; }

    section {
      margin-top: 22px;
      background: var(--surface);
      border: 1px solid var(--line);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      padding: 24px;
    }

    .faq-list { display: grid; gap: 12px; }

    details {
      border: 1px solid var(--line);
      border-radius: 10px;
      padding: 12px;
      background: #fbfdfb;
    }

    summary {
      font-weight: 700;
      cursor: pointer;
    }

    .contact-box {
      padding: 14px;
      background: #f5fbf7;
      border: 1px solid #d6ecde;
      border-radius: 10px;
    }

    footer {
      margin-top: 28px;
      border-top: 1px solid var(--line);
      padding: 22px 0;
      font-size: 0.94rem;
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

<section id="faq">
  <h2>FAQ</h2>
  <div class="faq-list">
    <details>
      <summary>Playback not working?</summary>
      <p>Reconnect Spotify and check your internet.</p>
    </details>
  </div>
</section>

<section id="contact">
  <h2>Contact</h2>
  <div class="contact-box">
    <strong>Email:</strong>
    <a href="mailto:support@spotiguess.com">support@spotiguess.com</a>
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
