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
    @media (max-width: 760px) {
      .nav {
        flex-direction: column;
        gap: 10px;
        align-items: flex-start;
      }

      .menu {
        flex-wrap: wrap;
        gap: 8px;
        padding-left: 0;
        margin: 0;
      }
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
  Spoti Guesser is a social music card game app built for people who love discovering songs, testing their music memory, and creating memorable game nights with friends and family. The idea is simple but powerful: turn Spotify music into playable QR cards, scan a card, start the track, and let everyone guess the song title, artist, and release year. It combines the energy of a party game with the personal touch of your own playlists, so every round feels unique to your group.
  </p> 
  <p>
  What makes Spoti Guesser special is how flexible it is. You can use it as a quick casual game in the living room, as a competitive challenge at parties, or as a custom trivia format for birthdays and events. If you connect Spotify, you unlock richer playback features and support for additional playlist scenarios. If you prefer not to connect, you can still enjoy core gameplay in guest-style flows. This means the app is welcoming to both dedicated Spotify users and players who just want a fun and easy game experience.
  </p> 
  <p>
  The app is designed around a full play loop: generate cards from a Spotify playlist, album, or track, export and print your cards, scan during gameplay, and verify answers with card back information. You can create a polished set of cards for repeated use, making Spoti Guesser feel like a real tabletop game with the convenience of a mobile app. Whether your group loves nostalgic classics, pop hits, indie gems, or themed playlists, the game adapts to your music taste instead of forcing a fixed catalog.
  </p> 
  <p>
  Spoti Guesser is also built with accessibility and usability in mind. The app supports multiple languages and is focused on straightforward navigation, clear actions, and quick setup so you can spend less time configuring and more time playing. From first launch to first scan, the goal is to keep everything intuitive: connect if you want, generate if you need, and start the game in seconds.
  </p> 
  <p>
    At its heart, Spoti Guesser is a passion project created by two students who wanted to bring people together through music, competition, and shared memories. It is made for laughter, debate, surprise discoveries, and those “I can’t believe you guessed that” moments. If your ideal game night includes great songs and friendly rivalry, Spoti Guesser was made for you.</p>
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
      <summary>What is Spoti Guesser?</summary>
      <p>Spoti Guesser is a music card game app where you scan QR cards and players guess the artist, title, and year.</p>
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
      <p>Go to Generate QR Codes, paste a Spotify link (playlist, album, or track), and export your cards as a PDF.</p>
    </details>

    <details>
      <summary>Which Spotify links are supported?</summary>
      <p>Links to playlists, albums, and individual tracks are supported.</p>
    </details>

    <details>
      <summary>Can I use private playlists?</summary>
      <p>Yes, but only if you are logged into Spotify and have access to that private playlist.</p>
    </details>

    <details>
      <summary>Why does the app request camera access?</summary>
      <p>The camera is required to scan QR codes on the game cards.</p>
    </details>

    <details>
      <summary>The QR code doesn’t scan, what should I do?</summary>
      <p>Make sure there is enough light, hold your camera steady, and check that the print is sharp and not damaged.</p>
    </details>

    <details>
      <summary>Playback is not working, what can I do?</summary>
      <p>Check your internet connection, log back into Spotify, and try scanning again.</p>
    </details>

    <details>
      <summary>Can I print cards?</summary>
      <p>Yes, you can export cards and print them on paper or cardstock for physical game nights.</p>
    </details>

    <details>
      <summary>Why do colors sometimes look different when printed?</summary>
      <p>Colors may vary due to screen settings, printer profiles, paper, and ink. Always test with a sample print first.</p>
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
      <p>For questions, feedback, or bugs, you can email BWBBstudio@gmail.com.</p>
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

<a href="https://www.paypal.com/paypalme/JSmeerkaas"
   target="_blank"
   rel="noopener noreferrer"
   class="btn">
  Donate via PayPal
</a>
  </div>
</section>

<section id="contact">
  <h2>Contact</h2>
  <p>
    You can contact us with e-mail, we normally respond within 24-28 hours.
  </p>
  <p>Email: <a href="mailto:BWBBstudio@gmail.com">BWBBstudio@gmail.com</a></p>
</section>

</main>

<footer>
  <p>© 2026 Spoti Guesser</p>
</footer>

</body>
</html>
