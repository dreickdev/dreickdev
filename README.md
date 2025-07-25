[![Banner de Perfil](https://github.com/Davekibh/Davekibh/blob/main/Images/Banner%20Image.png)](https://github.com/Erick-Conde)

<h1 align="center" style="font-family:'Orbitron'; color:#00ffc3;">🚀 Joselito Conde · <i>Creative Tech Engineer</i> 👨‍💻</h1>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Orbitron&size=22&pause=1000&color=00FFC3&center=true&vCenter=true&width=500&lines=Automatización+3D+%F0%9F%9A%80;Desarrollo+Mobile+%26+Backend+%F0%9F%94%A5;Electrónica+Creativa+%F0%9F%9A%BF;IA+y+Sistemas+Inteligentes+%F0%9F%A7%A0" alt="Typing SVG" />
</p>

---

<img align="right" src="https://media.giphy.com/media/dWesBcTLavkZuG35MI/giphy.gif" width="420" height="260" alt="Coder animado"/>

### 👾 ¿Quién soy?

Soy un **ingeniero creativo** que une código, hardware y diseño para **crear el futuro**.

- 🧠 Automatización 3D + electrónica + software
- 💡 Experiencias digitales únicas y funcionales
- 🛠️ Del backend a lo físico, integrando IA y control real

---

### 🌌 Lo que estoy creando ahora

- 🤖 Dispositivos físicos automatizados con Arduino/JS
- 📱 Apps móviles híbridas (Flutter / React Native)
- 🧬 Inteligencia artificial aplicada a procesos físicos
- 🎨 RGB shaders + visuales interactivos
- 🔌 Conectividad serial + bots + APIs inteligentes

---

### ⚙️ Mis herramientas de batalla

<p align="center">
  <img src="https://skillicons.dev/icons?i=js,nodejs,react,flutter,html,css,laravel,mysql,firebase,mongodb,arduino,threejs" />
</p>

---

### ✨ Proyectos principales

| 🌟 Proyecto | 🚀 Qué hace | 🧠 Tech Stack |
|------------|-------------|---------------|
| [`🌐 Fondo RGB Binario`](https://github.com/Erick-Conde/background-matrix-rgb) | Fondo Matrix con partículas RGB dinámicas | JS, Canvas |
| [`🤖 Robot 3D Automatizado`](https://github.com/Erick-Conde/robotica-3d) | Control físico con feedback 3D real | Arduino, JS |
| [`📦 Tienda Telegram`](https://github.com/Erick-Conde/tienda-telegram) | Sistema de pedidos con Telegram Bot | Node.js, SQL |
| [`🏫 Sistema Escolar`](https://github.com/Erick-Conde/sistema-escolar) | Administra clases, usuarios y notas | Laravel, MySQL |

---

### 📈 Stats cibernéticos

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Erick-Conde&show_icons=true&theme=tokyonight" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Erick-Conde&theme=tokyonight&layout=compact" />
</p>

---

### 🤖 Conecta conmigo

<p align="center">
  <a href="https://t.me/erick_conde"><img src="https://img.shields.io/badge/Telegram-00ffc3?style=for-the-badge&logo=telegram&logoColor=black"/></a>
  <a href="https://github.com/Erick-Conde"><img src="https://img.shields.io/badge/GitHub-00ffc3?style=for-the-badge&logo=github&logoColor=black"/></a>
  <a href="https://instagram.com/erickconde_dev"><img src="https://img.shields.io/badge/Instagram-ff00ff?style=for-the-badge&logo=instagram&logoColor=white"/></a>
  <a href="https://linkedin.com/in/erick-conde"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
</p>

---

### 🧬 Demo fondo RGB estilo Matrix

```html
<canvas id="matrix"></canvas>
<script>
  const canvas = document.getElementById("matrix");
  const ctx = canvas.getContext("2d");
  canvas.height = window.innerHeight;
  canvas.width = window.innerWidth;

  const binary = "01";
  const drops = Array(Math.floor(canvas.width / 20)).fill(1);

  function draw() {
    ctx.fillStyle = "rgba(0,0,0,0.05)";
    ctx.fillRect(0, 0, canvas.width, canvas.height);
    ctx.fillStyle = `hsl(${Math.random()*360},100%,70%)`;  // HSL color para efecto neón
    ctx.font = "20px monospace";
    for (let i = 0; i < drops.length; i++) {
      const text = binary[Math.floor(Math.random() * 2)];
      ctx.fillText(text, i * 20, drops[i] * 20);
      drops[i] = drops[i] * 20 > canvas.height || Math.random() > 0.95 ? 0 : drops[i] + 1;
    }
  }

  setInterval(draw, 50);
</script>
<style>
  body {
    margin: 0;
    background: black;
    overflow: hidden;
    font-family: 'Orbitron', sans-serif;
  }
  canvas {
    display: block;
  }
</style>
