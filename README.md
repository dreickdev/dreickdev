<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Developer Gamer</title>
  <style>
    html, body {
      margin: 0;
      padding: 0;
      overflow: hidden;
      background: black;
      color: white;
      font-family: 'Courier New', monospace;
    }

    canvas {
      position: fixed;
      top: 0;
      left: 0;
      z-index: -1;
    }

    .contenido {
      position: relative;
      z-index: 10;
      text-align: center;
      margin-top: 20vh;
      animation: glow 5s infinite alternate;
    }

    h1 {
      font-size: 3rem;
      color: white;
      text-shadow: 0 0 20px rgb(0,255,255);
    }

    p {
      font-size: 1.5rem;
      color: #00ffea;
    }

    button {
      background: none;
      border: 2px solid #00ffea;
      padding: 10px 20px;
      color: white;
      font-size: 1.2rem;
      margin-top: 20px;
      cursor: pointer;
      border-radius: 10px;
      transition: 0.3s;
      animation: glowBtn 4s infinite;
    }

    button:hover {
      background-color: rgba(0, 255, 255, 0.2);
    }

    @keyframes glow {
      0% {text-shadow: 0 0 10px red;}
      50% {text-shadow: 0 0 20px lime;}
      100% {text-shadow: 0 0 30px blue;}
    }

    @keyframes glowBtn {
      0% {box-shadow: 0 0 10px red;}
      50% {box-shadow: 0 0 20px lime;}
      100% {box-shadow: 0 0 30px blue;}
    }
  </style>
</head>
<body>
  <canvas id="lluviaBinaria"></canvas>

  <div class="contenido">
    <h1>¡Bienvenido, Desarrollador Gamer!</h1>
    <p>Tu experiencia: Automatización 3D, Backend y Apps Móviles</p>
    <button onclick="alert('¡Modo Dev Activado!')">Activar DevMode</button>
  </div>

  <script>
    const canvas = document.getElementById("lluviaBinaria");
    const ctx = canvas.getContext("2d");

    canvas.height = window.innerHeight;
    canvas.width = window.innerWidth;

    const letras = "01";
    const fontSize = 16;
    const columns = canvas.width / fontSize;

    const lluvia = Array(Math.floor(columns)).fill(1);

    function dibujar() {
      ctx.fillStyle = "rgba(0, 0, 0, 0.05)";
      ctx.fillRect(0, 0, canvas.width, canvas.height);

      ctx.fillStyle = `rgb(${Math.random()*255}, ${Math.random()*255}, ${Math.random()*255})`;
      ctx.font = fontSize + "px monospace";

      for (let i = 0; i < lluvia.length; i++) {
        const texto = letras[Math.floor(Math.random() * letras.length)];
        ctx.fillText(texto, i * fontSize, lluvia[i] * fontSize);

        if (lluvia[i] * fontSize > canvas.height && Math.random() > 0.975) {
          lluvia[i] = 0;
        }

        lluvia[i]++;
      }
    }

    setInterval(dibujar, 50);
  </script>
</body>
</html>
