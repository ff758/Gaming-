# Gaming-<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Simple Game</free fire>
  <style>
    body { text-align: center; font-family: sans-serif; }
    #game { width: 200px; height: 200px; margin: 20px auto; background: lightblue; }
  </style>
</head>
<body>
  <h1>Click the Box Game</h1>
  <p>Click the box to score!</p>
  <div id="game"></div>
  <p>Score: <span id="score">0</span></p>

  <script>
    let score = 0;
    const box = document.getElementById("game");
    const scoreDisplay = document.getElementById("score");

    box.addEventListener("click", () => {
      score++;
      scoreDisplay.textContent = score;
    });
  </script>
</body>
</html>
