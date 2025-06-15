<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>SM.Link Top Up</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to right, #000000, #1f1f1f);
      color: white;
    }header {
  background: linear-gradient(to right, red, blue);
  padding: 20px;
  text-align: center;
}

header h1 {
  margin: 0;
  font-size: 2.5rem;
  color: #00ffcc;
}

.logo {
  width: 100px;
  height: auto;
  margin-top: 10px;
}

.games {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 30px;
  padding: 40px;
}

.game-card {
  background-color: #222;
  border-radius: 10px;
  padding: 20px;
  text-align: center;
  width: 200px;
  box-shadow: 0 0 15px rgba(255, 255, 255, 0.1);
  transition: transform 0.3s ease;
}

.game-card:hover {
  transform: scale(1.05);
}

.game-card img {
  width: 100px;
  height: auto;
}

.game-card h2 {
  margin: 15px 0 10px;
  font-size: 1.2rem;
}

.topup-btn {
  background-color: #00ccff;
  border: none;
  color: black;
  padding: 10px 20px;
  border-radius: 5px;
  cursor: pointer;
  font-weight: bold;
}

.payment-info {
  background-color: #111;
  padding: 30px;
  text-align: center;
  color: #ccc;
  font-size: 1rem;
}

.payment-info h3 {
  color: #00ffcc;
  margin-bottom: 10px;
}

.payment-form {
  max-width: 400px;
  margin: 0 auto;
  background-color: #1c1c1c;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 255, 204, 0.2);
}

.payment-form label {
  display: block;
  margin-bottom: 8px;
  color: #fff;
}

.payment-form input {
  width: 100%;
  padding: 10px;
  margin-bottom: 15px;
  border: none;
  border-radius: 5px;
}

.payment-form button {
  width: 100%;
  padding: 10px;
  background-color: #00ffcc;
  color: black;
  border: none;
  border-radius: 5px;
  font-weight: bold;
  cursor: pointer;
}

.success-message {
  max-width: 400px;
  margin: 20px auto;
  background-color: #144d4d;
  color: #ccffcc;
  padding: 15px;
  text-align: center;
  border-radius: 8px;
  display: none;
}

footer {
  background-color: #111;
  text-align: center;
  padding: 20px;
  font-size: 0.9rem;
  color: #888;
}

  </style>
</head>
<body>
  <header>
    <h1>SM.Link Top Up</h1>
  </header>  <section class="games">
    <div class="game-card">
      <img src="https://upload.wikimedia.org/wikipedia/commons/6/6c/Free_Fire_logo.png" alt="Free Fire" />
      <h2>Free Fire</h2>
      <button class="topup-btn">Top-Up Now</button>
    </div><div class="game-card">
  <img src="https://upload.wikimedia.org/wikipedia/commons/3/38/PUBG_logo.png" alt="PUBG" />
  <h2>PUBG</h2>
  <button class="topup-btn">Top-Up Now</button>
</div>

<div class="game-card">
  <img src="https://upload.wikimedia.org/wikipedia/en/5/5f/Clash_of_Clans_logo.png" alt="COC" />
  <h2>Clash of Clans</h2>
  <button class="topup-btn">Top-Up Now</button>
</div>

  </section>  <section class="payment-info">
    <h3>Send Payment To:</h3>
    <p><strong>Bkash / Nagad / Rocket:</strong> 01882430808</p>
    <p>After payment, submit the confirmation below.</p><div class="success-message" id="successMessage">
  ✅ Thank you! Your payment confirmation has been submitted.<br>
  📲 We’ll contact you via <a href="https://wa.me/8801882430808" style="color:#00ffcc; text-decoration:underline;">WhatsApp</a> shortly.
</div>

<div class="payment-form">
  <form action="https://formsubmit.co/maruf11012@gmail.com" method="POST" onsubmit="showSuccessMessage()">
    <input type="hidden" name="_redirect" value="https://sm.link.topup.success">

    <label for="name">Your Name</label>
    <input type="text" id="name" name="name" required />

    <label for="game">Game Name (Free Fire / PUBG / COC)</label>
    <input type="text" id="game" name="game" required />

    <label for="playerId">Player ID</label>
    <input type="text" id="playerId" name="playerId" required />

    <label for="trxId">Transaction ID</label>
    <input type="text" id="trxId" name="trxId" required />

    <button type="submit">Submit Payment Confirmation</button>
  </form>
</div>

  </section>  <footer>
    &copy; 2025 SM.Link Top Up. All rights reserved.
  </footer>  <script>
    function showSuccessMessage() {
      setTimeout(() => {
        document.getElementById('successMessage').style.display = 'block';
      }, 500);
    }
  </script></body>
</html>
