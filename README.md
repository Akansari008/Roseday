# Roseday
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Happy Rose Day</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
    body {
        margin: 0;
        height: 100vh;
        font-family: 'Segoe UI', sans-serif;
        background: linear-gradient(to bottom, #ff9a9e, #fad0c4);
        overflow: hidden;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .card {
        background: rgba(255, 255, 255, 0.85);
        padding: 30px;
        border-radius: 20px;
        text-align: center;
        max-width: 350px;
        box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        z-index: 2;
    }

    h1 {
        color: #d1004f;
        margin-bottom: 10px;
    }

    p {
        font-size: 16px;
        color: #444;
    }

    .rose {
        font-size: 50px;
        animation: pulse 2s infinite;
    }

    @keyframes pulse {
        0% { transform: scale(1); }
        50% { transform: scale(1.2); }
        100% { transform: scale(1); }
    }

    /* Falling roses */
    .flower {
        position: absolute;
        top: -50px;
        font-size: 30px;
        animation: fall linear infinite;
        opacity: 0.8;
    }

    @keyframes fall {
        to {
            transform: translateY(110vh) rotate(360deg);
        }
    }
</style>
</head>

<body>

<div class="card">
    <div class="rose">🌹</div>
    <h1>Happy Rose Day</h1>
    <p>
        Just like this rose,<br>
        you make my life beautiful,<br>
        colorful, and full of love ❤️
    </p>
    <p><strong>Forever Yours</strong></p>
</div>

<!-- Flowers -->
<script>
    for (let i = 0; i < 20; i++) {
        let flower = document.createElement("div");
        flower.className = "flower";
        flower.innerHTML = "🌹";
        flower.style.left = Math.random() * 100 + "vw";
        flower.style.animationDuration = (Math.random() * 5 + 5) + "s";
        document.body.appendChild(flower);
    }
</script>

</body>
</html>
