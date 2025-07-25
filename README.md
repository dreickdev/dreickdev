[![Banner de Perfil](https://github.com/Davekibh/Davekibh/blob/main/Images/Banner%20Image.png)](https://github.com/Erick-Conde)

<h2 align="center">¡Hola, soy Erick Conde! 👋</h2>

🎓 Soy Desarrollador con experiencia en automatización 3D, desarrollo web backend y creación de apps móviles.  
💡 Apasionado por la innovación, los retos y la tecnología.  
🌐 Siempre aprendiendo y mejorando en cada proyecto.

---

<img align="right" src="https://media.giphy.com/media/dWesBcTLavkZuG35MI/giphy.gif" width="400" height="280" alt="Desarrollador animado"/>

### 🚀 Mi enfoque actual

- 🔭 Trabajando en proyectos 3D con automatización.
- 📱 Desarrollo de apps móviles (React Native, Flutter).
- 💻 Backend con Node.js, Laravel y APIs REST.
- ⚙️ Explorando inteligencia artificial y automatización avanzada.
- 🎨 Experimentos visuales con efectos RGB dinámicos y shaders.

---

<details>
<summary><strong>🛠️ Tecnologías & Herramientas</strong></summary>
<br/>

<p>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/html/html.png" height="20" alt="HTML"/>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/css/css.png" height="20" alt="CSS"/>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/javascript/javascript.png" height="20" alt="JavaScript"/>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/react/react.png" height="20" alt="React"/>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/nodejs/nodejs.png" height="20" alt="Node.js"/>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/flutter/flutter.png" height="20" alt="Flutter"/>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/firebase/firebase.png" height="20" alt="Firebase"/>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/mongodb/mongodb.png" height="20" alt="MongoDB"/>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/mysql/mysql.png" height="20" alt="MySQL"/>
  <img src="https://raw.githubusercontent.com/github/explore/main/topics/threejs/threejs.png" height="20" alt="Three.js"/>
</p>
</details>

---

<details>
<summary><strong>✨ Proyectos destacados</strong></summary>

- [Generador de fondos con partículas RGB y lluvia binaria](https://github.com/Erick-Conde/background-matrix-rgb)
- [Automatización 3D con controles físicos](https://github.com/Erick-Conde/robotica-3d)
- [Plataforma de pedidos online con Telegram Bot](https://github.com/Erick-Conde/tienda-telegram)
- [Sistema de control escolar](https://github.com/Erick-Conde/sistema-escolar)

</details>

---

<details>
<summary><strong>📊 Estadísticas de GitHub</strong></summary>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Erick-Conde&show_icons=true&theme=radical" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Erick-Conde&theme=radical&layout=compact" />
</p>

</details>

---

<details>
<summary><strong>📬 Conecta conmigo</strong></summary>

<p align="left">
  <a href="https://t.me/erick_conde"><img src="https://web.telegram.org/img/logo_share.png" width="22" alt="Telegram"/></a>
  <a href="https://github.com/Erick-Conde"><img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" width="22" alt="GitHub"/></a>
  <a href="https://instagram.com/erickconde_dev"><img src="https://upload.wikimedia.org/wikipedia/commons/a/a5/Instagram_icon.png" width="22" alt="Instagram"/></a>
  <a href="https://linkedin.com/in/erick-conde"><img src="https://cdn3.iconfinder.com/data/icons/inficons/512/linkedin.png" width="22" alt="LinkedIn"/></a>
</p>

</details>

---

### 🎨 Fondo animado con binarios

Para un fondo animado con "lluvia binaria" y efectos RGB, puedes añadir este archivo HTML en tu portafolio:

html
<canvas id="matrix"></canvas>
<script>
  const canvas = document.getElementById("matrix");
  const ctx = canvas.getContext("2d");

  canvas.height = window.innerHeight;
  canvas.width = window.innerWidth;

  const binary = "01";
  const columns = canvas.width / 20;
  const drops = Array(Math.floor(columns)).fill(1);

  function draw() {
    ctx.fillStyle = "rgba(0, 0, 0, 0.05)";
    ctx.fillRect(0, 0, canvas.width, canvas.height);

    ctx.fillStyle = `rgb(${Math.random()*255},${Math.random()*255},${Math.random()*255})`;
    ctx.font = "20px monospace";

    for (let i = 0; i < drops.length; i++) {
      const text = binary[Math.floor(Math.random() * binary.length)];
      ctx.fillText(text, i * 20, drops[i] * 20);
      drops[i] = (drops[i] * 20 > canvas.height || Math.random() > 0.95) ? 0 : drops[i] + 1;
    }
  }

  setInterval(draw, 50);
</script>
<style>
  body {
    margin: 0;
    background: black;
    overflow: hidden;
  }
  canvas {
    display: block;
  }
</style>    mejorar esta  pagina de git , quiero cambiuiar mi  ama
