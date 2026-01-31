
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>For Nim 🤍</title>
  <style>
    * { box-sizing: border-box; }

    body {
      margin: 0;
      font-family: 'Helvetica Neue', Arial, sans-serif;
      background: linear-gradient(135deg, #ffdde1, #ee9ca7);
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
      color: #333;
      text-align: center;
      overflow: hidden;
    }

    .card {
      background: white;
      padding: 40px 28px;
      border-radius: 24px;
      box-shadow: 0 20px 40px rgba(0,0,0,0.15);
      max-width: 360px;
      width: 90%;
      position: relative;
      z-index: 2;
    }

    h1 {
      font-size: 1.9rem;
      margin-bottom: 12px;
    }

    p {
      font-size: 1.05rem;
      line-height: 1.5;
      margin-bottom: 28px;
    }

    .heart {
      font-size: 2.2rem;
      margin-bottom: 18px;
    }

    button {
      padding: 14px 26px;
      border: none;
      border-radius: 30px;
      background: #e91e63;
      color: white;
      font-size: 1rem;
      font-weight: bold;
      cursor: pointer;
      transition: transform 0.2s ease, background 0.2s ease;
    }

    button:hover {
      background: #d81b60;
      transform: scale(1.05);
    }

    .message {
      display: none;
      margin-top: 25px;
      font-size: 1.1rem;
      font-weight: 500;
    }

    .photos {
      display: flex;
      gap: 10px;
      justify-content: center;
      margin-bottom: 22px;
    }

    .photos img {
      width: 90px;
      height: 90px;
      object-fit: cover;
      border-radius: 14px;
      box-shadow: 0 8px 16px rgba(0,0,0,0.15);
    }

    .floating-heart {
      position: absolute;
      font-size: 1.5rem;
      animation: floatUp 3s ease forwards;
      opacity: 0.9;
    }

    @keyframes floatUp {
      0% {
        transform: translateY(0) scale(1);
        opacity: 1;
      }
      100% {
        transform: translateY(-120px) scale(1.4);
        opacity: 0;
      }
    }
  </style>
</head>
<body>
  <div class="card">
    <div class="heart">🤍</div>
    <h1>Nim, my bunny…</h1>
  <p>
  Six Valentine’s together.
  <br />
  Not one and the same place together.
  <br /><br />
  But loving you from a distance has never changed how sure I am.
  <br />
  This is our last Valentine being apart.
</p>

    <div class="photos">
      <img src="photo1.jpg" alt="Us together" />
      <img src="photo2.jpg" alt="A favourite memory" />
      <img src="photo3.jpg" alt="My bunny" />
    </div>

    <button onclick="sayYes()">Yes, I’ll be your Valentine 💕</button>
    <div class="message" id="message">I knew it 🤍 I love you.</div>
  </div>

  <script>
  function sayYes() {
  const message = document.getElementById('message');
  message.style.display = 'block';

  const audio = document.getElementById('music');
  audio.volume = 0.7;
  audio.play();

  for (let i = 0; i < 15; i++) {
    createHeart();
  }
}
      const message = document.getElementById('message');
      message.style.display = 'block';

      for (let i = 0; i < 15; i++) {
        createHeart();
      }
    }

    function createHeart() {
      const heart = document.createElement('div');
      heart.className = 'floating-heart';
      heart.innerText = '🤍';
      heart.style.left = Math.random() * 100 + 'vw';
      heart.style.bottom = '0px';
      heart.style.animationDuration = 2 + Math.random() * 2 + 's';
      document.body.appendChild(heart);

      setTimeout(() => {
        heart.remove();
      }, 4000);
    }
  </audio https://music.apple.com/za/album/innerbloom/1058740883?i=1058740894
</body>
</html>
