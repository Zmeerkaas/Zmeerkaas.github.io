<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Spoti Guesser - Support</title>
  <meta name="description" content="Spoti Guesser is a music card game where you create and play your own Spotify-based party game." />

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

    body {
      margin: 0;
      font-family: Arial, sans-serif;
      color: var(--text);
      background:
        radial-gradient(1200px 500px at 20% -10%, #dff7e9 0%, transparent 60%),
        var(--bg);
    }

    .container {
      width: min(var(--maxw), 92vw);
      margin: auto;
    }

    header {
      background: white;
      border-bottom: 1px solid var(--line);
    }

    .nav {
      display: flex;
      justify-content: space-between;
      padding: 12px;
    }

    .brand {
      font-weight: bold;
      color: var(--brand);
    }

    .menu {
      display: flex;
      gap: 10px;
      list-style: none;
    }

    .menu a {
      text-decoration: none;
      padding: 6px 10px;
      border-radius: 999px;
    }

    .menu a:hover {
      background: var(--brand);
      color: white;
    }

    .hero {
      padding: 50px 0;
    }

    .hero-card {
      background: linear-gradient(135deg, #ffffff, #eafff2);
      padding: 30px;
      border-radius: var(--radius);
      box-shadow: var(--shadow);
    }

    .kicker {
      background: var(--brand);
      color: white;
      padding: 4px 10px;
      border-radius: 999px;
      font-size: 12px;
    }

    section {
      margin-top: 20px;
      background: white;
      padding: 20px;
      border-radius: var(--radius);
      border-left: 4px solid var(--brand);
    }

    .steps li {
      margin-bottom: 8px;
    }

    .faq-list details {
      margin-top: 10px;
      padding: 10px;
      border: 1px solid var(--line);
      border-radius: 8px;
    }

    .donate-box {
      background: #e9fff3;
      padding: 15px;
      border-radius: 10px;
      border: 1px solid #b7f0d1;
    }

    .btn {
      display: inline-block;
      margin-top: 10px;
      background: var(--brand);
      color: white;
      padding: 10px 14px;
      border-radius: 999px;
      text-decoration: none;
    }

    footer {
      text-align: center;
      margin: 30px 0;
      color: var(--muted);
    }
  </style>
</head>

<body>

<header>
  <nav class="container nav">
    <div class="brand">Spoti Guesser</div>
    <ul class="menu">
      <li><a href="#about">About</a></li>
      <li><a href="#how">How it works</a></li>
      <li><a href="#faq">FAQ</a></li>
      <li><a href="#support">Support</a></li>
      <li><a href="#donate">Support Us</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</header>

<div class="container hero">
  <div class="hero-card">
    <span class="kicker">The Music Card Game</span>
    <h1>Spoti Guesser</h1>
    <p>
      Turn your living room into a music quiz arena. Create your own card game using Spotify and challenge your friends.
    </p>
  </div>
</div>

<main class="container">

<section id="about">
  <h2>About the App</h2>
  <p>
    Spoti Guesser is a party game where you generate QR-code cards from Spotify songs and use them to play a real-life music guessing game.
  </p>
  <p>
    It’s inspired by games like Hitster, but lets you fully customize your own deck using your favorite playlists.
  </p>
  <p>
    Built as a passion project by two students:
    <br />Joris (development) & Tim (design).
  </p>
</section>

<section id="how">
  <h2>How it Works</h2>
  <ol class="steps">
    <li>Generate QR cards from a Spotify playlist</li>
    <li>Print them and write song info on the back</li>
    <li>Scan cards during the game</li>
    <li>Guess the song, artist, or year</li>
  </ol>
</section>

<section id="faq">
  <h2>FAQ</h2>
  <div class="faq-list">
    <details>
      <summary>Do I need Spotify?</summary>
      <p>Spotify is optional, but required for playback features.</p>
    </details>
    <details>
      <summary>Can I play without Spotify?</summary>
      <p>Yes, you can use guest mode, but with fewer features.</p>
    </details>
    <details>
      <summary>Playback not working?</summary>
      <p>Reconnect Spotify and check your internet connection.</p>
    </details>
  </div>
</section>

<section id="support">
  <h2>Support</h2>
  <p>
    Having issues? Try reconnecting Spotify, updating the app, or restarting your device.
  </p>
</section>

<section id="donate">
  <h2>Support Us ❤️</h2>
  <div class="donate-box">
    <p>
      Spoti Guesser is a student project. If you enjoy it, consider supporting development.
    </p>

    <!-- vervang link -->
    <a href="https://paypal.me/yourlink" target="_blank" class="btn">
      Donate via PayPal
    </a>
  </div>
</section>

<section id="contact">
  <h2>Contact</h2>
  <p>Email: <a href="mailto:BWBBstudio@gmail.com">BWBBstudio@gmail.com</a></p>
</section>

</main>

<footer>
  <p>© 2026 Spoti Guesser</p>
</footer>

</body>
</html>
