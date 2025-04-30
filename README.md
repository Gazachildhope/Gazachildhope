<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Help Gaza's Children</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #fff;
      color: #333;
    }

    header {
      background-color: #111;
      color: white;
      padding: 20px;
      text-align: center;
    }

    .logo {
      font-size: 1.4rem;
      font-weight: bold;
    }

    .section {
      padding: 40px 20px;
      max-width: 800px;
      margin: auto;
      line-height: 1.7;
    }

    .donate-btn {
      display: inline-block;
      background-color: #c0392b;
      color: white;
      padding: 12px 20px;
      border: none;
      border-radius: 8px;
      font-size: 1rem;
      cursor: pointer;
      margin-top: 20px;
    }

    .wallet-container {
      margin-top: 15px;
      display: none;
      background-color: #f4f4f4;
      padding: 15px;
      border-radius: 8px;
      text-align: center;
      font-family: monospace;
    }

    .wallet-container input {
      width: 90%;
      font-size: 1rem;
      padding: 8px;
      margin-top: 10px;
    }

    .icon-row {
      display: flex;
      justify-content: center;
      margin-top: 40px;
      gap: 20px;
    }

    .icon-row a img {
      width: 28px;
    }

    footer {
      text-align: center;
      padding: 20px;
      background-color: #eee;
      font-size: 0.9rem;
      margin-top: 40px;
    }
  </style>
  <script>
    function toggleWallet() {
      const wallet = document.getElementById('walletBox');
      wallet.style.display = wallet.style.display === 'block' ? 'none' : 'block';
    }

    function copyWallet() {
      const input = document.getElementById("walletInput");
      input.select();
      input.setSelectionRange(0, 99999);
      document.execCommand("copy");
      alert("Wallet address copied!");
    }
  </script>
</head>
<body>

<header>
  <div class="logo">Hope Beyond Rubble</div>
</header>

<div class="section">
  <p>
    I’ve walked the dusty streets of Gaza, where buildings once full of life now lie shattered. Children sift through rubble, not for toys—but for bread, for shoes, for a memory of safety. Hunger gnaws at their faces, and plastic sheets stretched across twisted metal are the only shelter they have. If you've never seen a toddler sleep on cold concrete next to a burned-out car, you don't yet know what helplessness means.
  </p>

  <p>
    Your donation isn't charity—it's rescue. Each 10 USDT brings food, clean water, or medical aid directly into the hands of those who need it most.
  </p>

  <button class="donate-btn" onclick="toggleWallet()">Donate Now</button>

  <div id="walletBox" class="wallet-container">
    <p>USDT (TRC20) Wallet Address:</p>
    <input type="text" id="walletInput" value="TN6vQfPgbzam9EuBMtBYTxEPjbxWscvXD4" readonly />
    <br/>
    <button class="donate-btn" style="background-color:#27ae60;" onclick="copyWallet()">Copy</button>
  </div>
</div>

<div class="section">
  <h2>How We Use Your Donations</h2>
  <p>
    Donations are used to purchase essential food supplies, basic medical kits, tents for shelter, and hygiene packs. We collaborate with local networks inside Gaza to ensure aid reaches real families. Every coin makes a difference—directly and immediately.
  </p>
</div>

<div class="section">
  <h2>About Us</h2>
  <p>
    Ethan Morgan, a volunteer aid coordinator and humanitarian advocate, leads this project with a team of global volunteers. With no overhead costs and no intermediaries, our focus is pure: helping children who’ve lost everything. Transparency is our promise.
  </p>
</div>

<div class="section">
  <h2>Contact</h2>
  <div class="icon-row">
    <a href="https://instagram.com/gazachildhope" target="_blank">
      <img src="https://upload.wikimedia.org/wikipedia/commons/e/e7/Instagram_logo_2016.svg" alt="Instagram" />
    </a>
    <a href="mailto:gazachildhope@gmail.com">
      <img src="https://upload.wikimedia.org/wikipedia/commons/4/4e/Gmail_Icon.png" alt="Email" />
    </a>
  </div>
</div>

<footer>
  &copy; 2025 GazaChildHope.org — All rights reserved.
</footer>

</body>
</html>
