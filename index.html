<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Jogo do Dinossauro</title>

  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      background: #f7f7f7;
      font-family: Arial, sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    #game {
      width: 800px;
      height: 300px;
      background: white;
      border: 2px solid #333;
      position: relative;
      overflow: hidden;
    }

    #ground {
      position: absolute;
      bottom: 40px;
      width: 100%;
      height: 3px;
      background: #333;
    }

    #dino {
      width: 45px;
      height: 55px;
      background: #444;
      position: absolute;
      left: 80px;
      bottom: 43px;
      border-radius: 5px;
    }

    /* Olho do dinossauro */
    #dino::before {
      content: "";
      width: 6px;
      height: 6px;
      background: white;
      position: absolute;
      right: 8px;
      top: 8px;
      border-radius: 50%;
    }

    #cactus {
      width: 25px;
      height: 50px;
      background: green;
      position: absolute;
      right: -30px;
      bottom: 43px;
    }

    #score {
      position: absolute;
      right: 20px;
      top: 15px;
      font-size: 20px;
      font-weight: bold;
    }

    #message {
      position: absolute;
      width: 100%;
      text-align: center;
      top: 100px;
      font-size: 25px;
      font-weight: bold;
      display: none;
    }

    #instructions {
      position: absolute;
      width: 100%;
      text-align: center;
      bottom: 5px;
      font-size: 14px;
      color: #555;
    }
  </style>
</head>

<body>

<div id="game">

  <div id="score">
    Pontos: 0
  </div>

  <div id="message">
    GAME OVER
    <br>
    <small>Pressione Espaço para reiniciar</small>
  </div>

  <div id="dino"></div>

  <div id="cactus"></div>

  <div id="ground"></div>

  <div id="instructions">
    Pressione ESPAÇO ou ↑ para pular
  </div>

</div>

<script>

const dino = document.getElementById("dino");
const cactus = document.getElementById("cactus");
const scoreElement = document.getElementById("score");
const message = document.getElementById("message");

let dinoY = 0;
let velocityY = 0;

let jumping = false;
let gameOver = false;

let cactusX = 800;

let score = 0;

let speed = 6;

const gravity = 0.8;
const jumpForce = 15;


// Função para pular
function jump() {

  if (!jumping && !gameOver) {

    velocityY = jumpForce;

    jumping = true;

  }

}


// Detectar teclado
document.addEventListener("keydown", function(event) {

  if (
    event.code === "Space" ||
    event.code === "ArrowUp"
  ) {

    event.preventDefault();

    if (gameOver) {

      restartGame();

    } else {

      jump();

    }

  }

});


// Também permite clicar para pular
document.addEventListener("click", function() {

  if (gameOver) {

    restartGame();

  } else {

    jump();

  }

});


// Verificar colisão
function checkCollision() {

  const dinoRect =
    dino.getBoundingClientRect();

  const cactusRect =
    cactus.getBoundingClientRect();


  if (

    dinoRect.right >
    cactusRect.left + 5 &&

    dinoRect.left <
    cactusRect.right - 5 &&

    dinoRect.bottom >
    cactusRect.top + 5

  ) {

    endGame();

  }

}


// Finalizar jogo
function endGame() {

  gameOver = true;

  message.style.display = "block";

}


// Reiniciar
function restartGame() {

  gameOver = false;

  score = 0;

  speed = 6;

  cactusX = 800;

  dinoY = 0;

  velocityY = 0;

  jumping = false;

  message.style.display = "none";

  scoreElement.innerText =
    "Pontos: 0";

}


// Loop principal do jogo
function gameLoop() {

  if (!gameOver) {

    // Movimento do dinossauro

    if (jumping) {

      dinoY += velocityY;

      velocityY -= gravity;


      if (dinoY <= 0) {

        dinoY = 0;

        velocityY = 0;

        jumping = false;

      }

    }


    dino.style.bottom =
      (43 + dinoY) + "px";


    // Movimento do cactus

    cactusX -= speed;


    if (cactusX < -40) {

      cactusX = 800 +
        Math.random() * 300;

      score++;

      scoreElement.innerText =
        "Pontos: " + score;


      // Aumenta a velocidade
      // conforme o jogador pontua

      if (score % 5 === 0) {

        speed += 0.5;

      }

    }


    cactus.style.left =
      cactusX + "px";


    checkCollision();

  }


  requestAnimationFrame(gameLoop);

}


// Iniciar jogo
gameLoop();

</script>

</body>
</html>
