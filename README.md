[![Banner de Perfil](https://github.com/Davekibh/Davekibh/blob/main/Images/Banner%20Image.png)](https://github.com/Erick-Conde)

<h1 align="center">🚀 Joselito Conde · <i>Creative Tech Engineer</i> 👨‍💻</h1>

<p align="center">
🎯 Automatización 3D · 💡 Innovación Tecnológica · 📱 Mobile & Backend Developer  
</p>

---

<img align="right" src="https://media.giphy.com/media/dWesBcTLavkZuG35MI/giphy.gif" width="420" height="260" alt="Coder animado"/>

### 👾 ¿Quién soy?

Soy un **desarrollador técnico-creativo** que fusiona hardware, software y diseño para dar vida a soluciones impactantes. Desde **automatización 3D** hasta sistemas inteligentes con IA, me enfoco en crear experiencias tecnológicas funcionales y futuristas.

🔧 Me destaco por:
- Resolver problemas reales con tecnología personalizada.
- Liderar y aprender en equipo.
- Mantener enfoque, agilidad y visión a largo plazo.

---

### 🌌 En qué estoy trabajando ahora

- 🤖 Control físico 3D automatizado
- 📲 Aplicaciones móviles inteligentes (React Native, Flutter)
- 🧠 Backend escalable (Node.js, Laravel, APIs REST)
- 🎮 Visuales experimentales RGB / efectos shaders
- 🧬 Exploración de IA + electrónica aplicada

---

<details>
<summary><strong>⚙️ Herramientas favoritas</strong></summary>
<br/>
<p>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/html/html.png" height="22" alt="HTML"/>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/css/css.png" height="22" alt="CSS"/>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/javascript/javascript.png" height="22" alt="JavaScript"/>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/react/react.png" height="22" alt="React"/>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/flutter/flutter.png" height="22" alt="Flutter"/>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/nodejs/nodejs.png" height="22" alt="Node.js"/>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/laravel/laravel.png" height="22" alt="Laravel"/>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/firebase/firebase.png" height="22" alt="Firebase"/>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/mongodb/mongodb.png" height="22" alt="MongoDB"/>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/mysql/mysql.png" height="22" alt="MySQL"/>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/arduino/arduino.png" height="22" alt="Arduino"/>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/threejs/threejs.png" height="22" alt="Three.js"/>
</p>
</details>

---

### ✨ Proyectos que representan mi estilo

| 🔗 Proyecto | 💬 Descripción breve | 🧠 Tecnologías |
|------------|----------------------|----------------|
| [🌐 Fondo RGB Binario](https://github.com/Erick-Conde/background-matrix-rgb) | Canvas animado con partículas RGB y efectos matrix | JS, Canvas, RGB |
| [🦾 Automatización Física 3D](https://github.com/Erick-Conde/robotica-3d) | Control de dispositivos físicos impresos en 3D | Arduino, JS, Serial COM |
| [🛒 Tienda Telegram](https://github.com/Erick-Conde/tienda-telegram) | Sistema de pedidos conectado a Telegram | Node.js, MySQL, Bot API |
| [🏫 Sistema Escolar](https://github.com/Erick-Conde/sistema-escolar) | Control de alumnos y materias con backend completo | Laravel, MySQL |

---

### 📈 Stats que importan

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Erick-Conde&show_icons=true&theme=tokyonight" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Erick-Conde&theme=tokyonight&layout=compact" />
</p>

---

### 🌐 Conecta conmigo

<p align="left">
  <a href="https://t.me/erick_conde"><img src="https://img.shields.io/badge/Telegram-0088cc?style=for-the-badge&logo=telegram&logoColor=white"/></a>
  <a href="https://github.com/Erick-Conde"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/></a>
  <a href="https://instagram.com/erickconde_dev"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"/></a>
  <a href="https://linkedin.com/in/erick-conde"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
</p>

---

### 🎨 Animación RGB Binaria (fragmento HTML demo)

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
    ctx.fillStyle = `rgb(${Math.random()*255},${Math.random()*255},${Math.random()*255})`;
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
  body { margin: 0; background: black; overflow: hidden; }
  canvas { display: block; }
</style>
