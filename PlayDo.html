<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>PlayDo Arcade</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Arial', sans-serif; }
    body { background: black; color: white; text-align: center; }
    header { background: red; padding: 20px; font-size: 24px; font-weight: bold; }
    .game-list { display: grid; grid-template-columns: 1fr; gap: 20px; padding: 20px; }
    iframe { width: 100%; height: 440px; border: 3px solid red; border-radius: 10px; }
    .game-box { background: #1a1a1a; padding: 10px; border-radius: 12px; box-shadow: 0 0 10px red; }
  </style>
</head>
<body>

  <header>🎮 Welcome to PlayDo 🎮</header>

  <div class="game-list">

    <!-- TIC TAC TOE -->
    <div class="game-box">
      <h2>Tic Tac Toe (vs AI)</h2>
      <iframe srcdoc="
        <style>
          body { background: black; color: white; text-align: center; font-family: sans-serif; }
          table { margin: 20px auto; border-collapse: collapse; }
          td { width: 80px; height: 80px; font-size: 36px; border: 2px solid red; cursor: pointer; }
          button { padding: 10px 20px; background: red; color: white; border: none; font-size: 16px; }
        </style>
        <table id='board'></table>
        <button onclick='reset()'>Play Again</button>
        <script>
          const board = document.getElementById('board');
          let cells = [];

          function createBoard() {
            board.innerHTML = '';
            cells = [];
            for (let i = 0; i < 3; i++) {
              const row = board.insertRow();
              cells[i] = [];
              for (let j = 0; j < 3; j++) {
                const cell = row.insertCell();
                cell.onclick = () => makeMove(i, j);
                cells[i][j] = cell;
              }
            }
          }

          function makeMove(i, j) {
            if (cells[i][j].textContent) return;
            cells[i][j].textContent = 'X';
            if (checkWin('X')) return alert('You win!');
            aiMove();
            if (checkWin('O')) return alert('AI wins!');
          }

          function aiMove() {
            for (let i = 0; i < 3; i++)
              for (let j = 0; j < 3; j++)
                if (!cells[i][j].textContent) return cells[i][j].textContent = 'O';
          }

          function checkWin(p) {
            for (let i = 0; i < 3; i++)
              if (cells[i][0].textContent === p && cells[i][1].textContent === p && cells[i][2].textContent === p) return true;
            for (let j = 0; j < 3; j++)
              if (cells[0][j].textContent === p && cells[1][j].textContent === p && cells[2][j].textContent === p) return true;
            if (cells[0][0].textContent === p && cells[1][1].textContent === p && cells[2][2].textContent === p) return true;
            if (cells[0][2].textContent === p && cells[1][1].textContent === p && cells[2][0].textContent === p) return true;
            return false;
          }

          function reset() { createBoard(); }
          createBoard();
        </script>
      "></iframe>
    </div>

    <!-- CAR RACING WITH OBSTACLES -->
    <div class="game-box">
      <h2>Car Racing (with Obstacles)</h2>
      <iframe srcdoc="
        <style>
          canvas { background: #111; display: block; margin: auto; border: 2px solid red; }
          .controls { margin-top: 10px; }
          button {
            background: red; color: white; padding: 10px 20px;
            margin: 5px; font-size: 18px; border: none; border-radius: 6px;
          }
        </style>
        <canvas id='carCanvas' width='300' height='400'></canvas>
        <div class='controls'>
          <button onclick='moveLeft()'>⬅ Left</button>
          <button onclick='moveRight()'>Right ➡</button>
        </div>
        <button onclick='location.reload()'>Play Again</button>
        <script>
          const canvas = document.getElementById('carCanvas');
          const ctx = canvas.getContext('2d');
          const roadWidth = 300;
          let carX = 135;
          let carY = 340;
          const carWidth = 30, carHeight = 50;
          let obstacles = [];
          let speed = 5;
          let gameOver = false;

          function drawCar() {
            ctx.fillStyle = 'red';
            ctx.fillRect(carX, carY, carWidth, carHeight);
          }

          function drawObstacles() {
            ctx.fillStyle = 'white';
            for (let obs of obstacles) {
              ctx.fillRect(obs.x, obs.y, carWidth, carHeight);
              obs.y += speed;

              // Collision check
              if (
                obs.x < carX + carWidth &&
                obs.x + carWidth > carX &&
                obs.y < carY + carHeight &&
                obs.y + carHeight > carY
              ) {
                gameOver = true;
              }
            }
            // Remove off-screen
            obstacles = obstacles.filter(obs => obs.y < 400);
          }

          function draw() {
            ctx.clearRect(0, 0, roadWidth, 400);
            drawCar();
            drawObstacles();

            if (Math.random() < 0.02) {
              const laneX = Math.floor(Math.random() * 10) * 30;
              obstacles.push({ x: laneX, y: -carHeight });
            }

            if (gameOver) {
              clearInterval(loop);
              alert('🚗 Crash! Game Over');
            }
          }

          function moveLeft() {
            if (carX > 0) carX -= 30;
          }

          function moveRight() {
            if (carX < roadWidth - carWidth) carX += 30;
          }

          const loop = setInterval(draw, 60);
        </script>
      "></iframe>
    </div>

  </div>
</body>
</html>
