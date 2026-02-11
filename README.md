<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>💙 te llegó una cartita by rocío 💙</title>
  <link href="https://fonts.googleapis.com/css2?family=Dancing+Script&family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: "Poppins", sans-serif;
      background-color: #fff;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
      text-align: center;
      color: #333;
      transition: background-color 0.5s ease;
    }
    h2 {
      margin-bottom: 20px;
    }
    .screen {
      display: none;
      animation: fadeIn 0.8s ease;
      width: 90%;
      max-width: 600px;
    }
    .active {
      display: block;
    }
    .main-img {
      width: 280px;
      height: auto;
      margin-bottom: 15px;
      cursor: pointer;
      transition: transform 0.3s ease;
      border: none;
      box-shadow: none;
    }
    .main-img:hover {
      transform: scale(1.05);
    }
    .card {
      background: repeating-linear-gradient(
        white,
        white 28px,
        #e3e3e3 29px
      );
      border-radius: 0; /* esquinas en punta */
      padding: 40px 60px;
      border: 2px solid #e5e5e5;
      width: 95%;
      max-width: 900px;
      text-align: left;
      margin: 0 auto;
      box-sizing: border-box;
      box-shadow: 0 0 15px rgba(0,0,0,0.1);
      animation: fadeIn 1s ease;
    }
    .card h3 {
      font-family: 'Dancing Script', cursive;
      font-size: 1.6em;
      text-align: left;
      margin-bottom: 10px;
      margin-left: 10px;
      color: #444;
    }
    .card p {
      font-family: 'Dancing Script', cursive;
      font-size: 1.15em;
      line-height: 1.2;
      text-align: justify;
      color: #444;
      margin: 10px 0;
    }
    .return-btn {
      margin-top: 25px;
      padding: 10px 20px;
      font-size: 1em;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      transition: 0.3s;
      background-color: #6d70bb;
      color: white;
    }
    .return-btn:hover {
      background-color: #6d70bb;
    }
    @keyframes fadeIn {
      from {opacity: 0; transform: scale(0.95);}
      to {opacity: 1; transform: scale(1);}
    }
  </style>
</head>
<body>
  <div class="screen active" id="screen1">
    <h2>Hola, te llegó una carta</h2>
    <img src="https://i.postimg.cc/rpjhwK3P/otter.png" alt="Correo" class="main-img" onclick="nextScreen(2)">
  </div>
  <div class="screen" id="screen2">
    <h2>Una cartita para ti</h2>
    <img src="https://i.postimg.cc/XvL2Ypmh/Screenshot_2026_02_11_at_01_05_32.png" alt="Carta" class="main-img" onclick="nextScreen(3)">
  </div>
  <div class="screen" id="screen3">
    <h2>¡Ábrela!</h2>
    <img src="https://i.postimg.cc/wB2Wj7Z4/carta_abierta.png" alt="Sobre" class="main-img" onclick="nextScreen(4)">
  </div>
  <div class="screen" id="screen4">
    <h2>¿Qué dirá?</h2>
    <img src="https://i.postimg.cc/GpKMmHVf/carta_con_texto.png" alt="Carta lista" class="main-img" onclick="nextScreen(5)">
  </div>
  <div class="screen" id="screen5">
    <div class="card">
    <h3>mi amadísimo Mitzio ฅ՞•ﻌ•՞ฅ ᢉ𐭩</h3>
      <p> Cada año que puedo acompañarte en estas fechas 
        lo agradezco profundamente, porque la vida contigo 
        tiene otros colores, es mas cálida, de tonos entre 
        naranja y rosados𓂃 ོ☼𓂃.</p>
      <p>Uno siempre siente que la vida va perdiendo colores
        a medida que crece pero contigo es lo contrario, 
        llegaste y revertiste ese efecto. Tus abrazos son 
        de verdad un rayito de sol⋆☀︎｡y tus ojos mi cafecito
        que necesito todas las mañanas⋆☕︎˖</p>
      <p>Te deseo lo mejor cada día y hoy no es la excepción
        eres una persona increíble, tierna, preocupada, sensible,
        amorosa, dulce, y te mereces todo lo que das de vuelta.</p>
      <p>Feliz cumpleaños mi wawito⋆✴︎˚｡⋆ 🎂  ༘⋆.</p> 
      <p>Gracias por llegar a este mundo y a mi vida,
        Gracias por nunca rendirte y seguir adelante día a día, 
        Gracias por encontrar un sonrisa siempre, y darle tus 
        colores y calidez al mundo.</p>
      <p>Te amo, de aquí al siguiente universo, a pasitos de tortuga 𓆉.</p>
      <p>Tuya, Rocío -`♡´-</p>
      <p>───────────୨ৎ───────────</p>
    </div>
    <div style="text-align: center;">
      <button class="return-btn" onclick="nextScreen(1)">🔙 Regresar</button>
    </div>
  </div>
  <script>
    function nextScreen(num) {
      const current = document.querySelector(".screen.active");
      if (current) current.classList.remove("active");
      document.getElementById("screen" + num).classList.add("active");
    }
  </script>
</body>
</html>
