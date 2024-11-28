<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>A Special Page for You</title>
    <style>
        body {
            font-family: 'Comic Sans MS', Arial, sans-serif;
            background: linear-gradient(135deg, #fbc2eb, #a6c1ee);
            color: #333;
            text-align: center;
            margin: 0;
            padding: 0;
            overflow: hidden;
        }
        h1 {
            font-size: 3rem;
            margin-top: 15vh;
        }
        p {
            font-size: 1.5rem;
            margin: 20px;
        }
        .heart {
            font-size: 5rem;
            color: red;
            animation: pulse 1.5s infinite;
            margin: 20px 0;
        }
        button {
            padding: 10px 20px;
            font-size: 1rem;
            background-color: #ff6f61;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        button:hover {
            background-color: #ff3e30;
        }
        .note {
            margin-top: 30px;
            font-style: italic;
            color: #555;
        }
        .footer {
            position: absolute;
            bottom: 10px;
            width: 100%;
            font-size: 0.9rem;
            color: #666;
        }
        @keyframes pulse {
            0%, 100% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.2);
            }
        }
        .stars {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            background: transparent;
            overflow: hidden;
        }
        .stars span {
            position: absolute;
            display: block;
            width: 5px;
            height: 5px;
            background: white;
            border-radius: 50%;
            animation: starAnimation 3s infinite;
        }
        @keyframes starAnimation {
            0% {
                transform: translateY(0) scale(0.5);
                opacity: 0.5;
            }
            50% {
                transform: translateY(-30px) scale(1);
                opacity: 1;
            }
            100% {
                transform: translateY(-60px) scale(0.5);
                opacity: 0.5;
            }
        }
    </style>
</head>
<body>
    <div class="stars">
        <!-- Add 50 small stars -->
        <script>
            for (let i = 0; i < 50; i++) {
                let star = document.createElement('span');
                star.style.top = Math.random() * 100 + 'vh';
                star.style.left = Math.random() * 100 + 'vw';
                star.style.animationDuration = (Math.random() * 2 + 2) + 's';
                star.style.animationDelay = Math.random() * 5 + 's';
                document.querySelector('.stars').appendChild(star);
            }
        </script>
    </div>
    <h1>Hello, natasha❤️</h1>
    <p>hi, just wanna wish happy working today. dont stress with your work and hope you always guarded by ALLAH.</p>
    <div class="heart">💖</div>
    <p class="note">PS: This page is as unique as you are, and I made it with all my heart. Every word here is meant just for you. 🥰</p>
    <button onclick="alert('i have a crush on you btw, but shy to confess :3 ')">Click Me</button>
    <div class="footer">
        <p>enjoy this web!. 💕</p>
    </div>
</body>
</html>
