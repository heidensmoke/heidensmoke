<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Telegram Web Game</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .game {
            text-align: center;
        }
        .btn {
            padding: 10px 20px;
            background-color: #3498db;
            color: white;
            border: none;
            cursor: pointer;
            font-size: 20px;
        }
        .btn:hover {
            background-color: #2980b9;
        }
    </style>
</head>
<body>
    <div class="game">
        <h1>Welcome to Hamster Combat!</h1>
        <button class="btn" onclick="startGame()">Start Game</button>
        <div id="result"></div>
    </div>

    <script>
        function startGame() {
            const damage = Math.floor(Math.random() * 10) + 1;
            document.getElementById('result').innerHTML = `You dealt ${damage} damage!`;
        }
    </script>
</body>
</html>
