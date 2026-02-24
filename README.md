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
        h1 { 
            text-transform: uppercase; 
            letter-spacing: 4px; 
            margin-bottom: 5px;
            font-size: 1.8rem;
        }
        .subtitle {
            font-style: italic;
            color: #888;
            margin-bottom: 20px;
            font-size: 0.9rem;
        }
        hr { border: 0; height: 1px; background: #333; margin: 20px 0; }
        ul { 
            list-style-type: none; 
            padding: 0; 
            text-align: left; 
            display: inline-block;
        }
        li { 
            padding: 8px 0;
            font-size: 1.1rem;
            border-bottom: 1px solid #222;
        }
        .play-btn {
            background-color: #d4af37;
            color: #121212;
            padding: 20px;
            border: none;
            font-weight: bold;
            border-radius: 50px;
            width: 100%;
            font-size: 1.2rem;
            cursor: pointer;
            margin-top: 30px;
            text-transform: uppercase;
            box-shadow: 0px 5px 15px rgba(212, 175, 55, 0.3);
            transition: transform 0.2s;
        }
        .play-btn:active { transform: scale(0.95); }
    </style>
</head>
<body>

    <div class="container">
        <h1>The Lion's Den</h1>
        <div class="subtitle">Timeline Shifting: JKD Roster 2.0</div>
        
        <hr>

        <ul>
            <li>🏆 Why am I financially independent?</li>
            <li>💪 Why am I in the best shape of my life?</li>
            <li>🥊 Why am I good at boxing?</li>
            <li>🏊 Why am I good at swimming?</li>
            <li>🔥 Why do I love to exercise?</li>
            <li>📈 Why am I successful at everything I do?</li>
            <li>🧘 Why am I kind, patient and calm?</li>
            <li>🕊️ Why am I slow to anger?</li>
            <li>✨ Why am I living the best version of myself?</li>
            <li>🌐 Why am I focused on my spatial awareness?</li>
        </ul>

        <audio id="askfirmationAudio">
            <source src="askfirmations101.mp3" type="audio/mpeg">
        </audio>

        <button class="play-btn" onclick="playAudio()">
            🔊 ACTIVATE ASKFIRMATIONS
        </button>
    </div>

    <script>
        function playAudio() {
            var audio = document.getElementById("askfirmationAudio");
            
            // diagnostic check to see if the element exists
            if (!audio) {
                alert("Technical Error: Audio element not found in code.");
                return;
            }

            audio.play().then(() => {
                console.log("Audio playing successfully.");
            }).catch((error) => {
                // The Safety Alert
                alert("DIAGNOSTIC: " + error.name + "\n\n1. Check if the file is named EXACTLY 'askfirmations101.mp3' on GitHub.\n2. Ensure your phone is NOT on silent mode.\n3. Tap the screen once before hitting play.");
            });
        }
    </script>

</body>
</html>
