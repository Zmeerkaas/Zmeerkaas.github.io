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
      --brand: #1DB954;
      --brand-dark: #159947;
      --radius: 14px;
      --shadow: 0 8px 28px rgba(16, 32, 24, 0.08);
      --maxw: 1040px;
    }

    * { box-sizing: border-box; }

    html, body {
      margin: 0;
      padding: 0;
      font-family: "Segoe UI", Arial, sans-serif;
      color: var(--text);
      background:
        radial-gradient(1200px 500px at 20% -10%, #dff7e9 0%, transparent 60%),
        radial-gradient(1000px 400px at 120% 10%, #eaf4ff 0%, transparent 60%),
        var(--bg);
    }

    a {
      color: var(--brand-dark);
      text-decoration: none;
    }

    a:hover { text-decoration: underline; }

    .container {
      width: min(var(--maxw), 92vw);
      margin: 0 auto;
    }

    header {
      position: sticky;
      top: 0;
      backdrop-filter: blur(8px);
      background: rgba(247, 250, 248, 0.9);
      border-bottom: 1px solid var(--line);
    }

    .nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 12px;
    }

    .brand {
      font-weight: 700;
      color: var(--brand);
    }

    .menu {
      list-style: none;
      display: flex;
      gap: 10px;
      padding: 0;
      margin: 0;
    }

    .menu a {
      padding: 8px 12px;
      border-radius: 999px;
      font-weight: 600;
    }

    .menu a:hover {
      background: var(--brand);
      color: white;
    }

    .hero {
      padding: 60px 0 20px;
    }

    .hero-card {
      background: linear-gradient(135deg, #ffffff, #f0fff6);
      border: 1px solid var(--line);
      border-radius: var(--radius);
      padding: 30px;
      box-shadow: var(--shadow);
    }

    .kicker {
      background: var(--brand);
      color: white;
      padding: 4px 10px;
      border-radius: 999px;
      font-size: 0.75rem;
      font-weight: 700;
    }

    h1 { margin: 10px 0; }

    section {
      margin-top: 20px;
      background: var(--surface);
      border-radius: var(--radius);
      padding: 22px;
      box-shadow: var(--shadow);
      border-left: 4px solid var(--brand);
    }

    .faq-list { display: grid; gap: 10px; }

    details {
      border: 1px solid var(--line);
      border-radius: 10px;
      padding: 10px;
      background: #fbfdfb;
    }

    summary { font-weight: 700; cursor: pointer; }

    .contact-box, .donate-box {
      padding: 14px;
      border-radius: 10px;
      background: #f5fbf7;
      border: 1px solid #d6ecde;
      margin-top: 10px;
    }

    .donate-box {
      background: linear-gradient(135deg, #e9fff3, #ffffff);
      border: 1px solid #b7f0d1;
    }

    .donate-btn {
      display: inline-block;
      margin-top: 10px;
      padding: 10px 16px;
      background: var(--brand);
      color: white;
      border-radius: 999px;
      font-weight: 600;
    }

    footer {
      margin-top: 30px;
      padding: 20px 0;
      text-align: center;
      color: var(--muted);
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
      <li><a href="#donate">Support Us</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</header>

<div class="container hero">
  <div class="hero-card">
    <span class="kicker">Official Support</span>
    <h1>Spoti Guesser</h1>
    <p>The Music Card Game — play with friends, scan QR cards and guess songs!</p>
  </div>
</div>

<main class="container">

<section id="about">
  <h2>About</h2>
  <p>
    Spoti Guesser is a music card game where you scan QR codes and guess the song, artist, and release year.
  </p>
  <p>
    You can generate your own cards using Spotify playlists, albums, or tracks and play with friends.
  </p>
</section>

<section id="support">
  <h2>Support & Help</h2>
  <p>Having issues? Try these steps:</p>
  <ul>
    <li>Reconnect Spotify in settings</li>
    <li>Check your internet connection</li>
    <li>Update the app to the latest version</li>
    <li>Restart the app or your device</li>
  </ul>
</section>

<section id="faq">
  <h2>FAQ</h2>
  <div class="faq-list">
    <details>
      <summary>Do I need Spotify?</summary>
      <p>Spotify is optional, but required for playback and private playlists.</p>
    </details>
    <details>
      <summary>Playback not working?</summary>
      <p>Reconnect Spotify and ensure your internet is stable.</p>
    </details>
    <details>
      <summary>How do I play?</summary>
      <p>Scan a QR code, listen to the music, and guess the song details.</p>
    </details>
  </div>
</section>

<section id="donate">
  <h2>Support Us ❤️</h2>
  <div class="donate-box">
    <p>
      Spoti Guesser is a passion project made by students. If you enjoy the app,
      you can support us with a small donation.
    </p>

    <!-- VERVANG DEZE LINK -->
    <a href="https://paypal.me/yourlink" target="_blank" class="donate-btn">
      Donate via PayPal
    </a>
  </div>
</section>

<section id="contact">
  <h2>Contact</h2>
  <div class="contact-box">
    <strong>Email:</strong><br />
    <a href="mailto:BWBBstudio@gmail.com">BWBBstudio@gmail.com</a>
  </div>
</section>

</main>

<footer>
  <p>© 2026 Spoti Guesser</p>
</footer>

</body>
</html>
