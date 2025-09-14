<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DOG DISCO Game</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Tone.js for the music -->
    <script src="https://unpkg.com/tone@14.7.58/build/Tone.js"></script>
    <style>
        @keyframes disco-lights {
            0% { 
                background: radial-gradient(circle, #8A2BE2, #4B0082); 
            }
            20% { 
                background: radial-gradient(circle, #FF1493, #C71585); 
            }
            40% { 
                background: radial-gradient(circle, #00FFFF, #008B8B); 
            }
            60% { 
                background: radial-gradient(circle, #FFD700, #DAA520); 
            }
            80% { 
                background: radial-gradient(circle, #32CD32, #228B22); 
            }
            100% { 
                background: radial-gradient(circle, #8A2BE2, #4B0082); 
            }
        }
        
        @keyframes sparkle-fall {
            0% {
                transform: translateY(-10vh) scale(0);
                opacity: 0;
            }
            10% {
                transform: translateY(0vh) scale(1);
                opacity: 1;
            }
            90% {
                opacity: 1;
            }
            100% {
                transform: translateY(110vh) scale(0.5);
                opacity: 0;
            }
        }

        @keyframes strobe-flash {
            0%, 50%, 100% { box-shadow: inset 0 0 0 0px rgba(0,0,0,0); }
            25% { box-shadow: inset 0 0 100px 50px rgba(255, 255, 0, 0.4); }
            75% { box-shadow: inset 0 0 100px 50px rgba(0, 255, 255, 0.4); }
        }

        @keyframes spotlight-rotate {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }

        @keyframes disco-ball-fall {
            from {
                transform: translateY(-100px);
                opacity: 1;
            }
            to {
                transform: translateY(100vh);
                opacity: 0;
            }
        }
        
        @keyframes jump-animation {
            0% { transform: translate(-50%, -50%); }
            50% { transform: translate(-50%, -100%); }
            100% { transform: translate(-50%, -50%); }
        }

        body {
            font-family: 'Inter', sans-serif;
            animation: disco-lights 8s infinite alternate, strobe-flash 2s linear infinite;
            overflow: hidden;
            touch-action: manipulation;
            position: relative;
        }
        
        body::before, body::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: 
                radial-gradient(circle, rgba(255,255,255,0.8) 1px, transparent 1px),
                radial-gradient(circle, rgba(255,255,255,0.8) 1px, transparent 1px);
            background-size: 50px 50px;
            background-position: 0 0, 25px 25px;
            animation: sparkle-fall 10s linear infinite;
            pointer-events: none;
        }

        body::after {
            animation-delay: -5s;
            background-size: 70px 70px;
            background-position: 10px 10px, 45px 45px;
        }

        .dancer {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            pointer-events: none;
        }

        .credit {
            position: absolute;
            bottom: 2rem;
            left: 50%;
            transform: translateX(-50%);
            color: white;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
            z-index: 10;
        }

        .spotlight {
            position: absolute;
            top: -50%;
            width: 150vw;
            height: 150vw;
            background: radial-gradient(circle at 50% 100%, rgba(255, 0, 255, 0.4), transparent 70%);
            opacity: 0.7;
            animation: spotlight-rotate 10s linear infinite;
            pointer-events: none;
            transform-origin: 50% 100%;
            z-index: 0;
        }
        .spotlight.left {
            left: -50%;
            animation-delay: 0s;
        }
        .spotlight.right {
            right: -50%;
            animation-delay: -5s;
        }

        .disco-ball {
            position: absolute;
            top: -50px;
            width: 30px;
            height: 30px;
            border-radius: 50%;
            background-color: #fff;
            box-shadow: 0 0 10px 5px #fff;
            animation: disco-ball-fall 5s linear forwards;
            pointer-events: none;
        }
        
        .message-box {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background-color: rgba(0, 0, 0, 0.7);
            color: white;
            padding: 1rem 2rem;
            border-radius: 1rem;
            font-size: 1.5rem;
            font-weight: bold;
            text-align: center;
            opacity: 0;
            transition: opacity 0.5s ease-in-out;
            pointer-events: none;
            z-index: 20;
        }

        #controls {
            display: flex;
            justify-content: center;
            gap: 1rem;
            margin-top: 2rem;
            z-index: 10;
        }

        .control-btn {
            background-color: #8A2BE2;
            color: white;
            padding: 1rem 2rem;
            border-radius: 9999px;
            font-size: 1.25rem;
            font-weight: bold;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
            transition: all 0.2s ease-in-out;
        }

        .control-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
        }
        .control-btn:active {
            transform: translateY(1px);
        }
    </style>
</head>
<body class="flex justify-center items-center h-screen relative flex-col">
    <!-- Spotlights -->
    <div class="spotlight left"></div>
    <div class="spotlight right"></div>

    <h1 class="text-4xl font-extrabold text-white text-shadow-lg">DOG DISCO</h1>
    <p class="text-xl text-white mb-8 text-shadow-lg">Help Alegro collect disco balls to win!</p>

    <div id="score" class="text-2xl text-white font-bold absolute top-4 left-4 z-10">Score: 0</div>
    
    <div id="message-box" class="message-box"></div>

    <div id="game-container" class="w-full h-full relative">
        <!-- The dancing character/element is now your image -->
        <div id="dancer" class="dancer w-48 h-48 rounded-full overflow-hidden shadow-lg z-10">
            <img 
                src="https://yabbering-teal-elytaoskby.edgeone.app/E929752F-5084-4589-8682-249B0EB2A325.jpeg.png"
                alt="The dancing character"
                class="w-full h-full object-cover"
            >
        </div>
        <button id="startButton" class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 bg-purple-500 hover:bg-purple-700 text-white font-bold py-4 px-8 rounded-full shadow-lg transition-all duration-300 transform scale-100 hover:scale-110">
            Start Disco!
        </button>
    </div>
    
    <div id="controls" class="hidden">
        <button id="leftBtn" class="control-btn">Left</button>
        <button id="jumpBtn" class="control-btn">Jump</button>
        <button id="rightBtn" class="control-btn">Right</button>
    </div>
    
    <div class="credit text-center p-4">
        <p class="font-semibold text-lg">created by ekaterina</p>
    </div>

    <script>
        let mainSynth = null;
        let barkSynth = null;
        let winningSynth = null;
        let gameInterval = null;
        let score = 0;
        let dancerX = 50; // Initial position in percentage
        let dancerY = 50; // Initial position in percentage

        const scoreElement = document.getElementById('score');
        const dancer = document.getElementById('dancer');
        const gameContainer = document.getElementById('game-container');
        const messageBox = document.getElementById('message-box');
        const startButton = document.getElementById('startButton');
        const controls = document.getElementById('controls');
        const leftBtn = document.getElementById('leftBtn');
        const rightBtn = document.getElementById('rightBtn');
        const jumpBtn = document.getElementById('jumpBtn');

        // Function to update dancer's position
        function updateDancerPosition() {
            dancer.style.left = `${dancerX}vw`;
            dancer.style.top = `${dancerY}vh`;
        }

        // Function to play a barking sound
        function playBarkSound() {
            barkSynth.triggerAttackRelease("A4", "8n");
            setTimeout(() => {
                barkSynth.triggerAttackRelease("G4", "8n");
            }, 100);
        }

        // Function to play a celebratory winning tune
        function playWinningSound() {
            winningSynth.triggerAttackRelease("C5", "8n");
            winningSynth.triggerAttackRelease("E5", "8n", "+0.2");
            winningSynth.triggerAttackRelease("G5", "8n", "+0.4");
        }

        // Function to create and drop a new disco ball
        function createDiscoBall() {
            const ball = document.createElement('div');
            ball.classList.add('disco-ball');
            ball.style.left = `${Math.random() * 95}vw`;
            const randomColor = `hsl(${Math.random() * 360}, 100%, 70%)`;
            ball.style.backgroundColor = randomColor;
            ball.style.boxShadow = `0 0 10px 5px ${randomColor}`;
            gameContainer.appendChild(ball);

            ball.addEventListener('animationend', () => {
                ball.remove();
            });
        }
        
        // Function to show a message in the message box
        function showMessage(text) {
            messageBox.textContent = text;
            messageBox.style.opacity = 1;
        }
        
        // Function to hide the message box
        function hideMessage() {
            messageBox.style.opacity = 0;
        }

        // Check for collisions with falling disco balls
        function checkCollisions() {
            const dancerRect = dancer.getBoundingClientRect();
            const discoBalls = document.querySelectorAll('.disco-ball');
            
            discoBalls.forEach(ball => {
                const ballRect = ball.getBoundingClientRect();

                // Simple collision detection
                if (dancerRect.x < ballRect.x + ballRect.width &&
                    dancerRect.x + dancerRect.width > ballRect.x &&
                    dancerRect.y < ballRect.y + ballRect.height &&
                    dancerRect.y + dancerRect.height > ballRect.y) {
                    
                    // Collision detected!
                    score++;
                    scoreElement.textContent = `Score: ${score}`;
                    ball.remove();
                    
                    if (score === 5) {
                        showMessage("ALEGRO IS A HAPPY DANCING DOG , GIVE HIM A TREAT .");
                        setTimeout(hideMessage, 4000); // Hide after 4 seconds
                        playBarkSound();
                    } else if (score === 10) {
                        showMessage("GIVE ALEGRO MONEY FOR TREATS !!!!!!!");
                        playBarkSound();
                    } else if (score === 15) {
                        showMessage("YOU WIN! ALEGRO IS THE KING OF MIND GAMES !");
                        setTimeout(hideMessage, 4000); // Hide after 4 seconds
                        playWinningSound();
                    }
                }
            });
        }

        // Main game loop
        function gameLoop() {
            checkCollisions();
            requestAnimationFrame(gameLoop);
        }

        // --- New button control functions ---
        leftBtn.addEventListener('click', () => {
            dancerX = Math.max(0, dancerX - 5);
            updateDancerPosition();
        });

        rightBtn.addEventListener('click', () => {
            dancerX = Math.min(95, dancerX + 5);
            updateDancerPosition();
        });
        
        jumpBtn.addEventListener('click', () => {
            dancer.style.animation = "jump-animation 0.5s ease-out";
            setTimeout(() => {
                dancer.style.animation = "";
            }, 500);
        });
        
        // This function will be called once when the start button is clicked
        startButton.addEventListener('click', () => {
            // Start the Tone.js audio context first, as browsers require user interaction
            Tone.start();

            // Main synth for the game disco melody
            mainSynth = new Tone.Synth({
                oscillator: { type: "square" }, 
                envelope: {
                    attack: 0.01,
                    decay: 0.1,
                    sustain: 0,
                    release: 0.1
                }
            }).toDestination();

            // The new "funny footsteps" style melody
            const melody = ["C3", "C2", "C3", "F2", "G3"];
            let melodyIndex = 0;

            Tone.Transport.scheduleRepeat(time => {
                const note = melody[melodyIndex];
                if (note) {
                    mainSynth.triggerAttackRelease(note, "8n", time);
                }
                melodyIndex = (melodyIndex + 1) % melody.length;
            }, "8n"); 

            // Synth for the barking sound
            barkSynth = new Tone.Synth({
                oscillator: { type: "sine" },
                envelope: {
                    attack: 0.01,
                    decay: 0.2,
                    sustain: 0.1,
                    release: 0.2
                }
            }).toDestination();

            // Synth for the winning sound
            winningSynth = new Tone.Synth({
                oscillator: { type: "square" },
                envelope: {
                    attack: 0.05,
                    decay: 0.5,
                    sustain: 0.1,
                    release: 0.5
                }
            }).toDestination();

            Tone.Transport.bpm.value = 180;
            Tone.Transport.start();
            
            // Start the game loop and remove the button
            startButton.style.display = 'none';
            controls.classList.remove('hidden');
            gameInterval = setInterval(createDiscoBall, 1500); // Slower interval
            gameLoop();
        });
    </script>
</body>
</html>
