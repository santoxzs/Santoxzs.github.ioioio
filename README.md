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
            overflow: hidden; /* Impede o conteúdo de sair da tela */
        }
        .container {
            text-align: center;
            background-color: rgba(255, 255, 255, 0.9); /* Fundo branco levemente transparente */
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            width: 90%;
            max-width: 500px;
            position: relative;
            z-index: 1;
        }
        .image-container img {
            width: 100%;
            max-width: 300px;
            border-radius: 10px;
            margin-bottom: 20px;
        }
        .content {
            background-color: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        h1 {
            font-size: 2.5rem;
            color: #e74c3c;
            text-shadow: 2px 2px 5px rgba(255, 255, 255, 0.5);
            font-family: 'Pacifico', cursive;
            animation: glow 1.5s ease-in-out infinite alternate;
        }
        .countdown {
            font-size: 2rem;
            margin-top: 20px;
            color: #2c3e50;
        }
        p {
            font-size: 1.5rem;
            color: #e74c3c;
            margin-top: 20px;
            text-shadow: 1px 1px 3px rgba(255, 255, 255, 0.5);
            font-family: 'Dancing Script', cursive;
        }
        .hearts {
            font-size: 3rem;
            color: red;
            margin-top: 20px;
            animation: heartbeat 1.5s ease-in-out infinite;
        }
        .sparkle {
            font-size: 2rem;
            color: #ffd700;
            animation: sparkle 1.5s infinite alternate;
        }
        /* Emojis distribuídos no fundo */
        .emoji {
            position: absolute;
            font-size: 3rem;
            z-index: 0;
            animation: float 6s ease-in-out infinite;
        }
        /* Corações */
        .emoji.heart1 { top: 10%; left: 10%; animation-delay: 0s; }
        .emoji.heart2 { top: 20%; right: 5%; animation-delay: 1s; }
        .emoji.heart3 { top: 50%; left: 20%; animation-delay: 2s; }
        .emoji.heart4 { bottom: 10%; right: 10%; animation-delay: 3s; }
        .emoji.heart5 { bottom: 20%; left: 5%; animation-delay: 4s; }
        .emoji.heart6 { top: 70%; left: 30%; animation-delay: 5s; }
        .emoji.heart7 { bottom: 30%; left: 10%; animation-delay: 6s; }
        .emoji.heart8 { top: 60%; right: 20%; animation-delay: 7s; }
        .emoji.heart9 { top: 40%; right: 15%; animation-delay: 8s; }
        .emoji.heart10 { bottom: 40%; left: 40%; animation-delay: 9s; }

        /* Animação de brilho */
        @keyframes sparkle {
            0% { opacity: 0.6; transform: scale(1); }
            50% { opacity: 1; transform: scale(1.1); }
            100% { opacity: 0.6; transform: scale(1); }
        }

        /* Animação de flutuar para os emojis */
        @keyframes float {
            0% { transform: translateY(0); opacity: 1; }
            50% { transform: translateY(-30px); opacity: 0.8; }
            100% { transform: translateY(0); opacity: 1; }
        }

        /* Efeito de brilho para o título */
        @keyframes glow {
            0% { text-shadow: 2px 2px 10px rgba(255, 255, 255, 0.5); }
            50% { text-shadow: 2px 2px 30px rgba(255, 255, 255, 1); }
            100% { text-shadow: 2px 2px 10px rgba(255, 255, 255, 0.5); }
        }

        /* Efeito de pulsação para os corações */
        @keyframes heartbeat {
            0% { transform: scale(1); }
            50% { transform: scale(1.2); }
            100% { transform: scale(1); }
        }

    </style>
</head>
<body>

<!-- Música do Spotify -->
<div class="container">
    <!-- Player Spotify embutido -->
    <iframe src="https://open.spotify.com/embed/track/5XeFesFbtLpXzIVDNQP22n" width="100%" height="380" frameborder="0" allow="encrypted-media"></iframe>

    <div class="image-container">
        <img src="https://github.com/santoxzs/Amor.html/blob/main/IMG-20241203-WA0007.jpg?raw=true" alt="Imagem do casal">
    </div>
    <div class="content">
        <h1>Dias Amando Você 🤍</h1>
        <div class="countdown" id="countdown"></div>
        <p>Você é tudo para mim, minha mulher da minha vida, eu te amarei para sempre, meu amor 🥺✨️</p>
        <div class="hearts">❤️🤍</div>
        <div class="sparkle">✨️</div>
    </div>
</div>

<!-- Emojis distribuídos pelo site -->
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
