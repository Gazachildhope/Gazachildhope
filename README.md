<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <meta name="description" content="Help Gaza's children by donating Tether (TRC20). Every donation counts towards providing emergency aid, food, and shelter to displaced children in Gaza." />
  <meta name="keywords" content="Gaza, children, donation, humanitarian aid, Tether, TRC20, emergency relief" />
  <meta property="og:title" content="Help Gaza's Children — Every Tether Counts" />
  <meta property="og:description" content="Your donation provides essential aid to children suffering in Gaza. Support them today." />
  <meta property="og:image" content="images/gaza-background.jpg" />
  <meta property="og:url" content="https://gazachildhope.github.io/Gazachildhope/" />
  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:title" content="Help Gaza's Children" />
  <meta name="twitter:description" content="Donate to support Gaza's children with your contribution today." />
  <meta name="twitter:image" content="images/gaza-background.jpg" />
  <title>Help Gaza's Children</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #f2f2f2;
      color: #333;
    }

    header {
      background-image: url('images/gaza-background.jpg');
      background-size: cover;
      background-position: center;
      height: 350px;
      display: flex;
      align-items: center;
      justify-content: center;
      color: white;
      text-shadow: 0px 0px 10px #000;
      text-align: center;
    }

    header h1 {
      font-size: 2.5rem;
      max-width: 90%;
    }

    .section {
      padding: 40px 20px;
      max-width: 900px;
      margin: auto;
    }

    .donation-box {
      background-color: #fff;
      padding: 25px;
      border-radius: 8px;
      box-shadow: 0px 2px 8px rgba(0,0,0,0.1);
      text-align: center;
    }

    .wallet-address {
      font-family: monospace;
      background-color: #eee;
      padding: 10px;
      border-radius: 5px;
      display: inline-block;
      margin: 10px 0;
    }

    .trust-section {
      background-color: #fafafa;
      padding: 40px 20px;
      margin-top: 20px;
    }

    .ethan {
      display: flex;
      align-items: center;
      gap: 20px;
      margin-top: 30px;
    }

    .ethan img {
      width: 120px;
      border-radius: 50%;
      box-shadow: 0px 2px 10px rgba(0,0,0,0.15);
    }

    footer {
      text-align: center;
      padding: 20px;
      background-color: #ddd;
      margin-top: 40px;
    }

    .qr {
      margin-top: 20px;
    }

    .qr img {
      width: 120px;
    }

    .donate-button {
      margin-top: 20px;
      padding: 15px 30px;
      background-color: #28a745;
      color: white;
      font-size: 1.2rem;
      border-radius: 5px;
      cursor: pointer;
      text-decoration: none;
    }

    .donate-button:hover {
      background-color: #218838;
    }

    .popup {
      position: absolute;
      top: 10%;
      left: 50%;
      transform: translateX(-50%);
      background-color: rgba(0, 0, 0, 0.7);
      color: white;
      padding: 20px;
      border-radius: 8px;
      display: none;
    }
  </style>
</head>
<body>

<header>
  <h1>Help Gaza's Children — Every Tether Counts</h1>
</header>

<div class="section">
  <div class="donation-box">
    <h2>Donate 10 USDT (TRC20)</h2>
    <p>Every 10 Tether helps provide emergency aid, food, and shelter to displaced children in Gaza.</p>
    <button class="donate-button" onclick="showWalletAddress()">Click to Copy Wallet Address</button>
    <div id="wallet-popup" class="popup">
      <p>Wallet Address: <span id="wallet-address">TN6vQfPgbzam9EuBMtBYTxEPjbxWscvXD4</span></p>
      <button onclick="copyToClipboard()">Copy Address</button>
    </div>
    <div class="qr">
      <img src="images/qr-code.png" alt="Donate QR Code">
    </div>
  </div>
</div>

<div class="trust-section">
  <h2>Why You Can Trust Us</h2>
  <p>This initiative is led by humanitarian volunteers and verified through full transparency. 100% of your donation goes directly to supporting affected families.</p>
  
  <div class="ethan">
    <img src="images/ethan.jpg" alt="Ethan Morgan">
    <div>
      <strong>Ethan Morgan</strong><br/>
      Founder & Volunteer Coordinator<br/>
      GazaChildHope.org
    </div>
  </div>
</div>

<footer>
  <p>Contact Us: <a href="mailto:contact@gazachildhope.org">contact@gazachildhope.org</a> | Follow us on <a href="https://www.instagram.com/gazachildhope">Instagram</a></p>
  &copy; 2025 GazaChildHope.org — All Rights Reserved.
</footer>

<script>
  function showWalletAddress() {
    document.getElementById("wallet-popup").style.display = "block";
  }

  function copyToClipboard() {
    const walletAddress = document.getElementById("wallet-address");
    const range = document.createRange();
    range.selectNode(walletAddress);
    window.getSelection().addRange(range);
    document.execCommand('copy');
    alert("Wallet Address Copied to Clipboard!");
  }
</script>

</body>
</html>
