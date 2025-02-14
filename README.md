<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dias Amando Você 🤍</title>
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&family=Pacifico&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #2e0044; /* Roxo escuro */
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            color: white;
            position: relative;
            overflow: hidden;
        }
        .container {
            text-align: center;
            background-color: rgba(255, 255, 255, 0.9); /* Fundo branco levemente transparente */
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            width: 90%;
            max-width: 1000px;
            position: relative;
            z-index: 1;
        }
        .image-container {
            display: flex;
            justify-content: space-between;
            gap: 10px;
            margin-bottom: 20px;
        }
        .image-container img {
            width: 100%;
            max-width: 220px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
        }
        .text-overlay {
            margin-top: 20px;
            font-family: 'Pacifico', cursive;
            font-size: 2rem;
            color: #e74c3c;
            text-shadow: 2px 2px 5px rgba(255, 255, 255, 0.5);
        }
        .countdown {
            font-size: 2rem;
            margin-top: 20px;
            color: #2c3e50;
        }
        .hearts {
            font-size: 2rem;
            color: red;
            margin-top: 20px;
        }
        .sparkle {
            font-size: 2rem;
            color: #ffd700;
        }
        /* Emojis distribuídos no fundo */
        .emoji {
            position: absolute;
            font-size: 3rem;
            z-index: 0;
        }
        /* Corações */
        .emoji.heart1 { top: 10%; left: 10%; }
        .emoji.heart2 { top: 20%; right: 5%; }
        .emoji.heart3 { top: 50%; left: 20%; }
        .emoji.heart4 { bottom: 10%; right: 10%; }
        .emoji.heart5 { bottom: 20%; left: 5%; }
        .emoji.heart6 { top: 70%; left: 30%; }
        .emoji.heart7 { bottom: 30%; left: 10%; }
        .emoji.heart8 { top: 60%; right: 20%; }
        .emoji.heart9 { top: 40%; right: 15%; }
        .emoji.heart10 { bottom: 40%; left: 40%; }

        /* Corações Brancos */
        .emoji.white1 { top: 30%; left: 50%; }
        .emoji.white2 { top: 70%; right: 10%; }
        .emoji.white3 { top: 60%; left: 40%; }
        .emoji.white4 { bottom: 20%; left: 40%; }
        .emoji.white5 { bottom: 5%; right: 20%; }
        .emoji.white6 { top: 10%; left: 80%; }
        .emoji.white7 { bottom: 30%; right: 5%; }
        .emoji.white8 { top: 50%; left: 60%; }
        .emoji.white9 { top: 80%; left: 20%; }
        .emoji.white10 { bottom: 10%; left: 70%; }

        /* Brilho */
        .emoji.sparkle1 { top: 40%; left: 10%; }
        .emoji.sparkle2 { top: 5%; right: 20%; }
        .emoji.sparkle3 { top: 80%; left: 30%; }
        .emoji.sparkle4 { bottom: 30%; right: 30%; }
        .emoji.sparkle5 { bottom: 40%; left: 50%; }
        .emoji.sparkle6 { top: 20%; left: 30%; }
        .emoji.sparkle7 { top: 60%; left: 10%; }
        .emoji.sparkle8 { bottom: 50%; left: 40%; }
        .emoji.sparkle9 { top: 70%; right: 15%; }
        .emoji.sparkle10 { bottom: 10%; left: 60%; }
    </style>
</head>
<body>

<!-- Emojis distribuídos -->
<div class="emoji heart1">❤️</div>
<div class="emoji heart2">❤️</div>
<div class="emoji heart3">❤️</div>
<div class="emoji heart4">❤️</div>
<div class="emoji heart5">❤️</div>
<div class="emoji heart6">❤️</div>
<div class="emoji heart7">❤️</div>
<div class="emoji heart8">❤️</div>
<div class="emoji heart9">❤️</div>
<div class="emoji heart10">❤️</div>

<div class="emoji white1">🤍</div>
<div class="emoji white2">🤍</div>
<div class="emoji white3">🤍</div>
<div class="emoji white4">🤍</div>
<div class="emoji white5">🤍</div>
<div class="emoji white6">🤍</div>
<div class="emoji white7">🤍</div>
<div class="emoji white8">🤍</div>
<div class="emoji white9">🤍</div>
<div class="emoji white10">🤍</div>

<div class="emoji sparkle1">✨️</div>
<div class="emoji sparkle2">✨️</div>
<div class="emoji sparkle3">✨️</div>
<div class="emoji sparkle4">✨️</div>
<div class="emoji sparkle5">✨️</div>
<div class="emoji sparkle6">✨️</div>
<div class="emoji sparkle7">✨️</div>
<div class="emoji sparkle8">✨️</div>
<div class="emoji sparkle9">✨️</div>
<div class="emoji sparkle10">✨️</div>

<div class="container">
    <div class="image-container">
        <img src="https://github.com/santoxzs/santoxzs.github.io/blob/main/IMG-20250128-WA0023.jpg?raw=true" alt="Imagem 1">
        <img src="https://github.com/santoxzs/Minha-quian-a-/blob/main/IMG_20241203_115037_136.jpg?raw=true" alt="Imagem 2">
        <img src="https://github.com/santoxzs/Minha-quian-a-/blob/main/IMG-20241211-WA0103.jpg?raw=true" alt="Imagem 3">
        <img src="https://github.com/santoxzs/Minha-quian-a-/blob/main/IMG-20241009-WA0024.jpg?raw=true" alt="Imagem 4">
    </div>
    <div class="text-overlay">
        Eu te amo muito minha mulher da minha vida 🤍✨️
    </div>
</div>

<script>
    const startDate = new Date("September 20, 2024 00:00:00").getTime();

    function updateCountdown() {
        const now = new Date().getTime();
        const timeDiff = now - startDate;

        const days = Math.floor(timeDiff / (1000 * 60 * 60 * 24));
        const hours = Math.floor((timeDiff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
        const minutes = Math.floor((timeDiff % (1000 * 60 * 60)) / (1000 * 60));
        const seconds = Math.floor((timeDiff % (1000 * 60)) / 1000);

        document.getElementById("countdown").innerHTML = `${days} dias, ${hours} horas, ${minutes} minutos e ${seconds} segundos`;
    }

    setInterval(updateCountdown, 1000);
</script>

</body>
</html>
