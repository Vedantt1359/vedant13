<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Our First Valentine 💕</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
body {
  margin: 0;
  font-family: 'Georgia', serif;
  background: linear-gradient(to bottom, #ffd6e8, #fff);
  text-align: center;
  color: #5a0c2f;
  overflow-x: hidden;
}

h1 {
  margin-top: 20px;
  font-size: 2.2em;
}

.container {
  max-width: 700px;
  margin: auto;
  padding: 20px;
}

.card {
  background: white;
  border-radius: 18px;
  padding: 25px;
  margin: 22px 0;
  box-shadow: 0 10px 25px rgba(0,0,0,0.12);
}

button {
  background: #ff4d88;
  color: white;
  border: none;
  padding: 12px 28px;
  border-radius: 30px;
  font-size: 1em;
  cursor: pointer;
}

button:hover {
  background: #e63e78;
}

.letter {
  display: none;
  text-align: left;
  line-height: 1.7;
  margin-top: 15px;
  animation: fadeIn 1.2s ease;
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(10px); }
  to { opacity: 1; transform: translateY(0); }
}

/* 💕 Heart Animation */
.heart {
  position: fixed;
  color: #ff5fa2;
  font-size: 24px;
  animation: floatUp 2.5s ease forwards;
}

@keyframes floatUp {
  0% { opacity: 1; transform: translateY(0) scale(1); }
  100% { opacity: 0; transform: translateY(-120px) scale(1.8); }
}

.footer {
  margin: 30px 0;
  font-size: 0.9em;
  opacity: 0.7;
}
</style>
</head>

<body>

<h1>💖 Our First Valentine Week 💖</h1>
<p>One letter. One day. Only for you 🌹</p>

<div class="container">

  <!-- TEMPLATE CARD -->
  <div class="card">
    <h2>🌹 Rose Day</h2>
    <button onclick="unlock('rose',7)">Unlock</button>
    <div class="letter" id="rose">
      <p><b>My Cutuuu Baby Girl 💕,</b></p>
      <p>
        On this Rose Day 🌹, I thought of giving you a rose to express my love…
        but then I realized no flower could ever compare to you.
        You are more beautiful than any rose,
        more gentle than its petals,
        and more precious than anything in this world.

        Every time I think of love, I think of you.
        You are the reason my heart smiles.
      </p>
      <p>Forever yours ❤️</p>
    </div>
  </div>

  <div class="card">
    <h2>💍 Propose Day</h2>
    <button onclick="unlock('propose',8)">Unlock</button>
    <div class="letter" id="propose">
      <p><b>My Love 💖,</b></p>
      <p>
        On Propose Day 💍, I want to propose to you—not just once,
        but again and again, every single day.
        Because every day I wake up,
        I choose you with my full heart.

        You are my safe place, my peace, my happiness.
        And today, like always
        I ask you Will you keep being mine, forever?
      </p>
      <p>Always choosing you 💕</p>
    </div>
  </div>

  <div class="card">
    <h2>🍫 Chocolate Day</h2>
    <button onclick="unlock('chocolate',9)">Unlock</button>
    <div class="letter" id="chocolate">
      <p><b>My Sweetest Girl 🍫,</b></p>
      <p>
        On Chocolate Day, I wish I could give you
        all the chocolates in the world…
        but honestly, none of them are as sweet as you.

       Your smile melts my heart,
       your words comfort my soul,
       and your love is my favorite sweetness.

       Loving you is the best treat life has given me.
      </p>
    </div>
  </div>

  <div class="card">
    <h2>🧸 Teddy Day</h2>
    <button onclick="unlock('teddy',10)">Unlock</button>
    <div class="letter" id="teddy">
      <p><b>My Teddy 🧸,</b></p>
      <p>
        Teddy Day reminds me of warmth and comfort,
        and it makes me wish I could be that teddy
        you hug tight every night.

        I want to be the one who makes you feel safe,
        loved, and protected—no matter what.
        In my heart, you’re always wrapped in my arms.
      </p>
    </div>
  </div>

  <div class="card">
    <h2>🤞 Promise Day</h2>
    <button onclick="unlock('promise',11)">Unlock</button>
    <div class="letter" id="promise">
      <p><b>My Forever 🤞,</b></p>
      <p>
        On Promise Day, I make this promise to you—
        I will stand with you in good times and bad,
        when life is easy and when it’s messy.

        I promise to grow with you,
        to learn from my mistakes,
        and to never stop loving you.

        My love may not be perfect,
        but it is real, honest, and true.
      </p>
    </div>
  </div>

  <div class="card">
    <h2>🤗😘 Hug & Kiss Day</h2>
    <button onclick="unlock('hug',13)">Unlock</button>
    <div class="letter" id="hug">
      <p><b>My Love 🤍,</b></p>
      <p>
        Your hug 🤗 makes everything feel okay
        without saying a single word.
        And your kiss 😘 makes my heart race
        and my whole day brighter.

        In your arms, I find home.
        In your love, I find peace.
 
        I wish I could hug you tighter
        and kiss you longer today.
      </p>
    </div>
  </div>

  <div class="card">
    <h2>❤️ Valentine’s Day</h2>
    <button onclick="unlock('valentine',14)">Unlock</button>
    <div class="letter" id="valentine">
      <p><b>My Valentine ❤️,</b></p>
      <p>
        Valentine’s Day is not just one day for me.
        For me, loving you is every single day.

        You are my best friend, my partner,
        my forever person.
        I want to grow with you, laugh with you,
        fight small fights and come back stronger.

        Thank you for loving me,
        for understanding me,
        and for staying with me.

        I dream of a future filled with
        late-night talks, silly moments,
        big dreams, and endless memories—
        all with you.
      </p>
    </div>
  </div>

</div>

<div class="footer">
  Made with endless love 💕
</div>

<script>
function unlock(id, unlockDay) {
  const now = new Date();
  const day = now.getDate();
  const month = now.getMonth(); // February = 1

  if (month === 1 && day >= unlockDay) {
    document.getElementById(id).style.display = "block";
    createHearts();
  } else {
    alert("⏳ This letter will unlock on " + unlockDay + " February 💖");
  }
}

function createHearts() {
  for (let i = 0; i < 18; i++) {
    const heart = document.createElement("div");
    heart.className = "heart";
    heart.innerHTML = "💗";
    heart.style.left = Math.random() * window.innerWidth + "px";
    heart.style.bottom = "0px";
    document.body.appendChild(heart);

    setTimeout(() => {
      heart.remove();
    }, 2500);
  }
}
</script>

</body>
</html>
