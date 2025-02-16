<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Download Games</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
            text-align: center;
        }
        .container {
            max-width: 1200px;
            margin: auto;
            padding: 20px;
        }
        .games {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            padding: 20px;
        }
        .game {
            background: white;
            padding: 15px;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        .game img {
            width: 100%;
            height: auto;
            border-radius: 10px;
        }
        .game h2 {
            font-size: 1.2em;
            margin: 10px 0;
        }
        .game p {
            font-size: 0.9em;
            color: #666;
        }
        .download-btn {
            display: inline-block;
            padding: 10px 15px;
            background: #007bff;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            margin-top: 10px;
        }
        .download-btn:hover {
            background: #0056b3;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Download Games</h1>
        <div class="games">
            <!-- Generating 100 game entries dynamically -->
            
            <script>
                let gamesContainer = document.querySelector('.games');
                for (let i = 1; i <= 100; i++) {
                    let gameDiv = document.createElement('div');
                    gameDiv.classList.add('game');
                    gameDiv.innerHTML = `
                        <img src="https://via.placeholder.com/250" alt="Game Image">
                        <h2>Game Title ${i}</h2>
                        <p>Description for game ${i} with exciting features.</p>
                        <a href="#" class="download-btn">Download Now</a>
                    `;
                    gamesContainer.appendChild(gameDiv);
                }
            </script>
        </div>
    </div>
</body>
</html>
