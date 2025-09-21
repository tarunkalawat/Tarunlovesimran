<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tarun ❤️ Simran</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Arial', sans-serif;
      text-align: center;
      color: #fff;
      background: url('https://i.ibb.co/TLmn5nM/red-roses.jpg') no-repeat center center/cover;
    }

    .overlay {
      background: rgba(0, 0, 0, 0.6);
      min-height: 100vh;
      padding: 20px;
    }

    h1 {
      font-size: 55px;
      margin-top: 40px;
      color: #ff3366;
      text-shadow: 2px 2px 10px black;
      animation: heartbeat 1.5s infinite;
    }

    @keyframes heartbeat {
      0% { transform: scale(1); }
      25% { transform: scale(1.2); }
      50% { transform: scale(1); }
      75% { transform: scale(1.2); }
      100% { transform: scale(1); }
    }

    p {
      font-size: 22px;
      margin-top: 20px;
      color: #ffd6d6;
      text-shadow: 1px 1px 5px black;
    }

    .heart {
      font-size: 90px;
      margin: 20px 0;
      animation: pulse 1.2s infinite;
    }

    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.3); }
      100% { transform: scale(1); }
    }

    .section {
      margin-top: 40px;
      padding: 20px;
      background: rgba(255, 51, 102, 0.3);
      border-radius: 20px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.4);
    }

    .section h2 {
      font-size: 30px;
      margin-bottom: 20px;
      color: #ffcccc;
      text-shadow: 1px 1px 5px black;
    }

    .text {
      font-style: italic;
      font-size: 20px;
      margin: 15px 0;
      animation: fadeIn 3s ease-in-out;
    }

    @keyframes fadeIn {
      from {opacity: 0;}
      to {opacity: 1;}
    }

    /* Buttons */
    .btns {
      margin-top: 30px;
    }
    button {
      background: #ff3366;
      color: white;
      border: none;
      padding: 12px 25px;
      margin: 10px;
      border-radius: 30px;
      font-size: 18px;
      cursor: pointer;
      transition: 0.3s;
      box-shadow: 0 4px 8px rgba(0,0,0,0.4);
    }
    button:hover {
      background: #e6004c;
      transform: scale(1.1);
    }

    /* Popup animation */
    .popup {
      position: absolute;
      font-size: 40px;
      animation: floatUp 2s forwards;
    }

    @keyframes floatUp {
      0% {opacity: 1; transform: translateY(0);}
      100% {opacity: 0; transform: translateY(-150px);}
    }
  </style>
</head>
<body>
  <div class="overlay">
    <h1>Tarun ❤️ Simran</h1>
    <div class="heart">💖</div>
    <p>Simran, tum meri rooh ka sabse khoobsurat hissa ho 🌹<br> Forever & Always – Tarun 💕</p>

    <!-- Quotes Section -->
    <div class="section">
      <h2>🌹 Love Quotes 🌹</h2>
      <div class="text">"Tum meri muskaan ho, jo har dukh mita deti hai."</div>
      <div class="text">"Meri zindagi ka sabse khoobsurat hissa ho tum, Simran."</div>
      <div class="text">"Har dhadkan mein sirf tum ho, aur hamesha rahogi."</div>
    </div>

    <!-- Shayari Section -->
    <div class="section">
      <h2>💖 Pyaar Bhari Shayariyan 💖</h2>
      <div class="text">“Tere bina adhuri hai zindagi meri,<br> Tum meri mohabbat ka sabse khoobsurat ehsaas ho.”</div>
      <div class="text">“Dil se nikli har dhadkan ka naam tum ho,<br> Tum meri dua, meri zindagi ho.”</div>
      <div class="text">“Chaand taare bhi sharma jaate hain dekh kar tumhe,<br> Simran, tum meri mohabbat ka geet ho.”</div>
    </div>

    <!-- Buttons -->
    <div class="btns">
      <button onclick="showPopup('❤️')">Send Heart</button>
      <button onclick="showPopup('💋')">Send Kiss</button>
    </div>
  </div>

  <script>
    function showPopup(symbol) {
      const popup = document.createElement("div");
      popup.className = "popup";
      popup.innerText = symbol;
      popup.style.left = (Math.random() * window.innerWidth) + "px";
      popup.style.top = (window.innerHeight - 100) + "px";
      document.body.appendChild(popup);

      setTimeout(() => {
        popup.remove();
      }, 2000);
    }
  </script>
</body>
</html>
