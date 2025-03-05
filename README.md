<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Will You Be Mine? ❤️</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: pink;
            flex-direction: column;
            font-family: Arial, sans-serif;
            text-align: center;
        }
        .heart {
            color: red;
            font-size: 50px;
            animation: heartbeat 1s infinite alternate;
        }
        @keyframes heartbeat {
            from { transform: scale(1); }
            to { transform: scale(1.2); }
        }
        .buttons {
            margin-top: 20px;
        }
        .button {
            background-color: red;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            font-size: 18px;
            cursor: pointer;
            margin: 10px;
            position: relative;
        }
    </style>
</head>
<body>
    <h1>Will You Be Mine Forever? ❤️</h1>
    <div class="heart">❤️</div>
    <div class="buttons">
        <button class="button" onclick="sayYes()">Yes</button>
        <button class="button" id="noButton" onclick="moveNoButton()">No</button>
    </div>
    <p id="message" class="hidden-message" style="display: none; font-size: 20px; color: darkred; margin-top: 20px;"></p>

    <script>
        function sayYes() {
            document.getElementById('message').innerText = 'Yay! I Love You So Much! 💖';
            document.getElementById('message').style.display = 'block';
        }

        function moveNoButton() {
            let button = document.getElementById('noButton');
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 50);
            button.style.position = 'absolute';
            button.style.left = x + 'px';
            button.style.top = y + 'px';
        }
    </script>
</body>
</html>
