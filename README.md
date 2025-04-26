# ¡Hola! 👋 Soy **Victor Vasquez** | Desarrollador Full Stack 🚀  

💻 Apasionado por el desarrollo web y la programación.  
🔍 Enfocado en crear soluciones innovadoras y eficientes.  
🚀 Siempre aprendiendo nuevas tecnologías.  

### 🛠️ Tecnologías y Herramientas  

<div align="center">  
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">  
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">  
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">  
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js">  
  <img src="https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white" alt="Rust">  
</div>  

### 📊 Estadísticas de GitHub  

<div align="center">  
  <img src="https://github-readme-stats.vercel.app/api?username=VictorVasquezZT2005&show_icons=true&theme=radical" alt="Estadísticas">  
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=VictorVasquezZT2005&layout=compact&theme=radical" alt="Lenguajes más usados">  
</div>  

### 🎮 ¡Juego Interactivo!  
Adivina un número entre **1 y 100**. Si aciertas, te felicitaré con un mensaje de éxito. ¡Vamos a jugar!  

```html
<div id="game-container">
  <h3>Juego: Adivina el Número</h3>
  <p>Ingresa un número entre 1 y 100:</p>
  <input type="number" id="guess" min="1" max="100">
  <button onclick="checkGuess()">¡Adivina!</button>
  <p id="result"></p>
</div>

<script>
  let randomNumber = Math.floor(Math.random() * 100) + 1;

  function checkGuess() {
    let userGuess = document.getElementById("guess").value;
    let resultText = document.getElementById("result");

    if (userGuess < randomNumber) {
      resultText.textContent = "¡Demasiado bajo! Intenta de nuevo.";
    } else if (userGuess > randomNumber) {
      resultText.textContent = "¡Demasiado alto! Intenta de nuevo.";
    } else {
      resultText.textContent = "¡Felicidades, acertaste!";
    }
  }
</script>

<style>
  #game-container {
    margin: 20px;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
    text-align: center;
  }
  input {
    margin: 10px 0;
    padding: 5px;
    font-size: 16px;
  }
  button {
    padding: 10px 15px;
    font-size: 16px;
    background-color: #4CAF50;
    color: white;
    border: none;
    cursor: pointer;
  }
  button:hover {
    background-color: #45a049;
  }
</style>
