<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Lion's Den</title>
    <style>
        body {
            background-color: #121212;
            color: #d4af37;
            font-family: 'Segoe UI', Helvetica, Arial, sans-serif;
            text-align: center;
            padding: 20px;
            margin: 0;
        }
        .container {
            border: 2px solid #d4af37;
            padding: 25px;
            border-radius: 20px;
            max-width: 450px;
            margin: 20px auto;
            background-color: #1a1a1a;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
        }
        h1 { text-transform: lowercase; letter-spacing: 2px; margin-bottom: 5px; font-size: 1.8rem; }
        .subtitle { font-style: italic; color: #888; margin-bottom: 20px; font-size: 0.9rem; text-transform: lowercase; }
        hr { border: 0; height: 1px; background: #333; margin: 20px 0; }
        ul { list-style-type: none; padding: 0; text-align: left; display: inline-block; }
        li { padding: 8px 0; font-size: 1.1rem; border-bottom: 1px solid #222; }
        
        .play-btn {
            background-color: #d4af37;
            color: #121212;
            padding: 22px;
            border: none;
            font-weight: bold;
            border-radius: 50px;
            width: 100%;
            font-size: 1.2rem;
            cursor: pointer;
            margin-top: 30px;
            text-transform: lowercase; /* Force the text to lowercase */
            box-shadow: 0px 5px 15px rgba(212, 175, 55, 0.3);
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% { box-shadow: 0 0 0 0 rgba(212, 175, 55, 0.7); }
            70% { box-shadow: 0 0 0 15px rgba(212, 175, 55, 0); }
            100% { box-shadow: 0 0 0 0 rgba(212, 175, 55, 0); }
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>the lion's den</h1>
        <div class="subtitle">timeline shifting: jkd roster 2.0</div>
        <hr>
        <ul>
            <li>🏆 why am i financially independent?</li>
            <li>💪 why am i in the best shape of my life?</li>
            <li>🥊 why am i good at boxing?</li>
            <li>🏊 why am i good at swimming?</li>
            <li>🔥 why do i love to exercise?</li>
            <li>📈 why am i successful at everything i do?</li>
            <li>🧘 why am i kind, patient and calm?</li>
            <li>🕊️ why am i slow to anger?</li>
            <li>✨ why am i living the best version of myself?</li>
            <li>🌐 why am i focused on my spatial awareness?</li>
        </ul>

        <audio id="askfirmationAudio">
            <source src="askfirmations101.mp3" type="audio/mpeg">
        </audio>

        <button class="play-btn" onclick="playAudio()">
            🔊 activate askfirmations 101
        </button>
    </div>

    <script>
        function playAudio() {
            var audio = document.getElementById("askfirmationAudio");
            audio.play().catch((error) => {
                alert("diagnostic: " + error.name + "\ncheck file name or silent switch.");
            });
        }
    </script>
</body>
</html>
