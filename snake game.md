---
layout: page
title: Snake Game
search_exclude: true
permalink: /snake game/
---



<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Snake Game</title>
    <style>
        html, body {
            margin: 0;
            padding: 0;
            height: 100%;
            background-color: #e9e9e9;
            display: flex;
            flex-direction: column;
        }

        #gameContainer {
            width: 100vw;
            height: 70vh;
            display: flex;
            justify-content: center;
            align-items: flex-end;
            position: relative;
        }

        canvas {
            background-image: url('https://www.transparenttextures.com/patterns/grass.png');
            background-size: cover;
            border: 2px solid #333;
            box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);
            border-radius: 10px;
        }

        #resetButton {
            display: none;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            margin: 20px;
            padding: 12px 25px;
            font-size: 18px;
            color: white;
            background-color: #007bff;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            transition: background-color 0.3s ease, transform 0.2s ease;
        }

        #resetButton:hover {
            background-color: #0056b3;
        }

        #resetButton:active {
            background-color: #003f88;
            transform: scale(0.98);
        }

        #gameOverText {
            display: none;
            position: absolute;
            top: 40%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-size: 48px;
            color: red;
            font-family: 'Arial Black', sans-serif;
            text-shadow: 2px 2px 4px #000;
        }

        body {
            overflow-y: scroll;
        }
    </style>
</head>
<body>

    <div id="gameContainer">
        <canvas id="snakeGame"></canvas>
        <div id="gameOverText">Game Over</div>
        <button id="resetButton">Try Again</button>
    </div>

    <script>
        const canvas = document.getElementById("snakeGame");
        const ctx = canvas.getContext("2d");

        const gameOverText = document.getElementById("gameOverText");
        const resetButton = document.getElementById("resetButton");

        canvas.width = Math.min(window.innerWidth * 0.8, 600);
        canvas.height = Math.min(window.innerHeight * 0.8, 600);

        const box = 40;
        const speed = 150;

        const canvasCols = Math.floor(canvas.width / box);
        const canvasRows = Math.floor(canvas.height / box);

        let snake, food, score, direction, game, isInvincible, powerUpActive, powerUpTimer;
        let powerUp;
        
        function initGame() {
            snake = [];
            snake[0] = { x: Math.floor(canvasCols / 2) * box, y: Math.floor(canvasRows / 2) * box };

            food = generateFood();
            powerUp = generateFood(); // Power-up has the same position format as food
            powerUpActive = false;

            score = 0;
            direction = null;
            isInvincible = false;
            powerUpTimer = 0;

            gameOverText.style.display = "none";
            resetButton.style.display = "none";
            clearInterval(game);
            game = setInterval(drawGame, speed);
        }

        function generateFood() {
            return {
                x: Math.floor(Math.random() * canvasCols) * box,
                y: Math.floor(Math.random() * canvasRows) * box,
            };
        }

        function setDirection(event) {
            if (event.keyCode === 37 && direction !== "RIGHT") direction = "LEFT";
            else if (event.keyCode === 38 && direction !== "DOWN") direction = "UP";
            else if (event.keyCode === 39 && direction !== "LEFT") direction = "RIGHT";
            else if (event.keyCode === 40 && direction !== "UP") direction = "DOWN";
        }

        function collision(newHead, array) {
            for (let i = 0; i < array.length; i++) {
                if (newHead.x === array[i].x && newHead.y === array[i].y) {
                    return true;
                }
            }
            return false;
        }

        function endGame() {
            clearInterval(game);
            gameOverText.style.display = "block";
            resetButton.style.display = "block";
        }

        function activatePowerUp() {
            isInvincible = true;
            powerUpActive = true;
            powerUpTimer = 10;
            setTimeout(() => {
                isInvincible = false;
                powerUpActive = false;
            }, 10000); // Power-up lasts for 10 seconds
        }

        function drawGame() {
            ctx.clearRect(0, 0, canvas.width, canvas.height);

            // Draw snake
            for (let i = 0; i < snake.length; i++) {
                ctx.fillStyle = (i === 0) ? (powerUpActive ? "gold" : "#333") : (powerUpActive ? "yellow" : "#4CAF50");
                ctx.beginPath();
                ctx.arc(snake[i].x + box / 2, snake[i].y + box / 2, box / 2, 0, 2 * Math.PI);
                ctx.fill();
                ctx.strokeStyle = "#FFF";
                ctx.stroke();
            }

            // Draw fruit (food)
            let fruitImage = new Image();
            fruitImage.src = 'https://img.icons8.com/ios/50/000000/apple--v1.png';
            ctx.drawImage(fruitImage, food.x, food.y, box, box);

            // Draw power-up occasionally
            if (Math.random() < 0.1 && !powerUpActive) {
                let powerUpImage = new Image();
                powerUpImage.src = 'https://img.icons8.com/emoji/48/000000/star-emoji.png';
                ctx.drawImage(powerUpImage, powerUp.x, powerUp.y, box, box);
            }

            let snakeX = snake[0].x;
            let snakeY = snake[0].y;

            if (direction === "LEFT") snakeX -= box;
            if (direction === "UP") snakeY -= box;
            if (direction === "RIGHT") snakeX += box;
            if (direction === "DOWN") snakeY += box;

            // Check if snake eats the food
            if (snakeX === food.x && snakeY === food.y) {
                score++;
                food = generateFood();
            } else {
                snake.pop();
            }

            // Check if snake collects the power-up
            if (snakeX === powerUp.x && snakeY === powerUp.y && !powerUpActive) {
                activatePowerUp();
                powerUp = generateFood(); // Move the power-up to a new location
            }

            let newHead = { x: snakeX, y: snakeY };

            // Check if snake hits the wall or collides with itself
            if (
                (snakeX < 0 || snakeY < 0 || snakeX >= canvas.width || snakeY >= canvas.height) && !isInvincible ||
                collision(newHead, snake)
            ) {
                endGame();
            }

            snake.unshift(newHead);

            ctx.fillStyle = "#000";
            ctx.font = "20px Arial";
            ctx.fillText("Score: " + score, 10, canvas.height - 20);
        }

        document.addEventListener("keydown", setDirection);

        window.addEventListener("keydown", (e) => {
            if (["ArrowUp", "ArrowDown", "ArrowLeft", "ArrowRight"].includes(e.key)) {
                e.preventDefault();
            }
        });

        resetButton.addEventListener("click", initGame);

        window.addEventListener("resize", function() {
            canvas.width = Math.min(window.innerWidth * 0.8, 600);
            canvas.height = Math.min(window.innerHeight * 0.8, 600);
        });

        initGame();
    </script>

</body>
</html>
