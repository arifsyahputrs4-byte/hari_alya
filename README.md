<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Kejutan dari Arif 💌</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500&family=Great+Vibes&family=Dancing+Script&display=swap');

    body {
      margin: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      background: linear-gradient(135deg, #ff9ac9, #ffd1dc);
      font-family: 'Poppins', sans-serif;
      overflow: hidden;
    }

    .container {
      text-align: center;
      background: #fff8fb;
      padding: 40px 30px;
      border-radius: 20px;
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
      max-width: 350px;
      width: 90%;
      animation: fadeIn 1s ease;
      transition: opacity 1s ease;
    }

    h1 {
      font-family: "Great Vibes", cursive;
      font-size: 34px;
      color: #ff4b9b;
      margin-bottom: 10px;
    }

    p {
      font-family: 'Dancing Script', cursive;
      font-size: 18px;
      color: #444;
      margin-bottom: 25px;
      line-height: 1.4em;
    }

    input {
      width: 100%;
      padding: 10px 12px;
      border: 2px solid #ff8fc6;
      border-radius: 10px;
      outline: none;
      font-size: 15px;
      margin-bottom: 15px;
      text-align: center;
      transition: 0.3s;
    }

    input:focus {
      border-color: #ff4b9b;
      box-shadow: 0 0 5px rgba(255, 75, 155, 0.4);
    }

    button {
      background: linear-gradient(90deg, #ff4b9b, #ff7bbd);
      color: white;
      border: none;
      padding: 12px 0;
      border-radius: 12px;
      font-size: 16px;
      cursor: pointer;
      transition: 0.3s;
      width: 100%;
    }

    button:hover {
      transform: scale(1.05);
      background: linear-gradient(90deg, #ff7bbd, #ff4b9b);
    }

    .hearts {
      font-size: 24px;
      margin: 10px 0;
      animation: float 2s infinite ease-in-out;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: scale(0.95); }
      to { opacity: 1; transform: scale(1); }
    }

    @keyframes float {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-8px); }
    }

    /* Halaman kejutan */
    .surprise {
      display: none;
      text-align: center;
      animation: fadeIn 1.5s ease forwards;
      color: #ff4b9b;
      font-family: 'Dancing Script', cursive;
    }

    .surprise h2 {
      font-size: 28px;
      margin-bottom: 10px;
    }

    .surprise p {
      font-size: 20px;
      color: #333;
    }

    .fade-out {
      opacity: 0;
      pointer-events: none;
    }
  </style>
</head>
<body>
  <div class="container" id="formBox">
    <h1>Hai, Alya 💕</h1>
    <div class="hearts">💖💞</div>
    <p>Masukkan nama dan kata sandi rahasiamu<br>untuk membuka kejutan spesial 💌</p>

    <input type="text" id="nama" placeholder="Masukkan namamu" />
    <input type="password" id="sandi" placeholder="Masukkan kata sandi" />
    <button onclick="bukaKejutan()">Buka Kejutan 💝</button>
  </div>

  <div class="surprise" id="surpriseBox">
    <h2>🎉 Hai Alya! 🎉</h2>
    <p>Terima kasih sudah membuka kejutan ini 💖<br>
    Kamu adalah sosok yang istimewa dan selalu membawa warna di hari Arif 🌸</p>
    <div style="font-size:28px; margin-top:15px;">💌💞🌷✨</div>
  </div>

  <script>
    function bukaKejutan() {
      const nama = document.getElementById("nama").value.trim();
      const sandi = document.getElementById("sandi").value.trim();
      const formBox = document.getElementById("formBox");
      const surpriseBox = document.getElementById("surpriseBox");

      if (nama && sandi) {
        formBox.classList.add("fade-out");
        setTimeout(() => {
          formBox.style.display = "none";
          surpriseBox.style.display = "block";
        }, 1000);
      } else {
        alert("Masukkan nama dan kata sandi dulu ya 💕");
      }
    }
  </script>
</body>
</html>

<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>🎉 Selamat Ulang Tahun 🎂</title>
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(135deg, #ffd1dc, #ffe4e1);
      height: 100vh;
      margin: 0;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      overflow: hidden;
    }
    h1 {
      color: #ff4d88;
      font-size: 28px;
      margin-top: 20px;
    }
    p {
      color: #555;
      font-size: 16px;
      max-width: 400px;
      margin: 10px auto 30px;
      line-height: 1.5;
    }
    .gallery {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
      justify-content: center;
      margin-bottom: 20px;
    }
    img {
      max-width: 250px;
      border-radius: 20px;
      box-shadow: 0 4px 20px rgba(0,0,0,0.2);
      transition: transform 0.3s ease;
    }
    img:hover {
      transform: scale(1.05);
    }
    button {
      background-color: #ff66a3;
      color: white;
      border: none;
      padding: 12px 24px;
      border-radius: 12px;
      font-size: 18px;
      cursor: pointer;
      transition: 0.3s;
      margin-top: 20px;
    }
    button:hover {
      background-color: #ff3385;
    }
    #content {
      display: none;
      animation: fadeIn 1s ease-in-out forwards;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>
  <button onclick="showSurprise()">🎁 Lihat Kejutan</button>

  <div id="content">
    <div class="gallery">
      <img src="IMG_0222.png" alt="Foto 1">
      <img src="IMG_0223.jpeg" alt="Foto 2">
    </div>
    <h1>🎉 Selamat Ulang Tahun Sayang ! 🎂</h1>
    <p>
      Semoga hari istimewa ini penuh tawa, kebahagiaan, dan cinta.  
      Teruslah menjadi pribadi yang baik, hangat, dan menginspirasi.  
      Semoga semua impianmu perlahan menjadi nyata 💖
    </p>
  </div>

  <script>
    function showSurprise() {
      document.querySelector("button").style.display = "none";
      document.getElementById("content").style.display = "block";
    }
  </script>
</body>
</html>
