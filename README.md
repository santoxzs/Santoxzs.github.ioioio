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
            position: relative;
        }
        .text-overlay {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-size: 3rem;
            color: white;
            font-family: 'Pacifico', cursive;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.7);
        }
        
        /* Emojis distribuídos no fundo */
        .emoji {
            position: absolute;
            font-size: 3rem;
            z-index: 0;
            animation: float 3s ease-in-out infinite;
        }
        /* Corações vermelhos */
        .emoji.heart1 { top: 10%; left: 10%; animation: floatUpDown 2s ease-in-out infinite; color: red; }
        .emoji.heart2 { top: 20%; right: 5%; animation: floatUpDown 3s ease-in-out infinite; color: red; }
        .emoji.heart3 { top: 50%; left: 20%; animation: floatUpDown 4s ease-in-out infinite; color: red; }
        .emoji.heart4 { bottom: 10%; right: 10%; animation: floatUpDown 2s ease-in-out infinite; color: red; }
        .emoji.heart5 { bottom: 20%; left: 5%; animation: floatUpDown 5s ease-in-out infinite; color: red; }
        .emoji.heart6 { top: 70%; left: 30%; animation: floatUpDown 3s ease-in-out infinite; color: red; }
        .emoji.heart7 { bottom: 30%; left: 10%; animation: floatUpDown 4s ease-in-out infinite; color: red; }
        .emoji.heart8 { top: 60%; right: 20%; animation: floatUpDown 6s ease-in-out infinite; color: red; }
        .emoji.heart9 { top: 40%; right: 15%; animation: floatUpDown 7s ease-in-out infinite; color: red; }
        .emoji.heart10 { bottom: 40%; left: 40%; animation: floatUpDown 8s ease-in-out infinite; color: red; }
        
        /* Corações brancos */
        .emoji.white-heart1 { top: 5%; left: 20%; animation: floatUpDown 3s ease-in-out infinite; color: white; }
        .emoji.white-heart2 { top: 15%; right: 10%; animation: floatUpDown 4s ease-in-out infinite; color: white; }
        .emoji.white-heart3 { top: 25%; left: 10%; animation: floatUpDown 6s ease-in-out infinite; color: white; }
        .emoji.white-heart4 { bottom: 15%; right: 20%; animation: floatUpDown 5s ease-in-out infinite; color: white; }
        .emoji.white-heart5 { bottom: 25%; left: 15%; animation: floatUpDown 7s ease-in-out infinite; color: white; }
        .emoji.white-heart6 { top: 60%; left: 30%; animation: floatUpDown 4s ease-in-out infinite; color: white; }
        .emoji.white-heart7 { bottom: 50%; left: 25%; animation: floatUpDown 3s ease-in-out infinite; color: white; }
        .emoji.white-heart8 { top: 80%; right: 20%; animation: floatUpDown 6s ease-in-out infinite; color: white; }
        .emoji.white-heart9 { top: 55%; left: 35%; animation: floatUpDown 4s ease-in-out infinite; color: white; }
        .emoji.white-heart10 { bottom: 30%; left: 40%; animation: floatUpDown 8s ease-in-out infinite; color: white; }

        /* Animação de flutuar para os emojis */
        @keyframes float {
            0% { transform: translateY(0); opacity: 1; }
            50% { transform: translateY(-30px); opacity: 0.8; }
            100% { transform: translateY(0); opacity: 1; }
        }

        /* Animação de subida e descida para os corações */
        @keyframes floatUpDown {
            0% { transform: translateY(0); }
            50% { transform: translateY(-20px); }
            100% { transform: translateY(0); }
        }
    </style>
</head>
<body>

<!-- Música do Spotify -->
<div class="container">
    <!-- Player Spotify embutido -->
    <iframe src="https://open.spotify.com/embed/track/5XeFesFbtLpXzIVDNQP22n" width="100%" height="380" frameborder="0" allow="encrypted-media"></iframe>

    <div class="image-container">
        <div class="image-item">
            <img src="https://github.com/santoxzs/santoxzs.github.io/blob/main/IMG-20250128-WA0023.jpg?raw=true" alt="Imagem 1">
            <div class="text-overlay">Eu</div>
        </div>
        <div class="image-item">
            <img src="https://github.com/santoxzs/Minha-quian-a-/blob/main/IMG_20241203_115037_136.jpg?raw=true" alt="Imagem 2">
            <div class="text-overlay">Te</div>
        </div>
        <div class="image-item">
            <img src="https://github.com/santoxzs/Minha-quian-a-/blob/main/IMG-20241211-WA0103.jpg?raw=true" alt="Imagem 3">
            <div class="text-overlay">Amo</div>
        </div>
        <div class="image-item">
            <img src="https://github.com/santoxzs/Minha-quian-a-/blob/main/IMG-20241009-WA0024.jpg?raw=true" alt="Imagem 4">
            <div class="text-overlay">Muito</div>
        </div>
    </div>
</div>

<!-- Emojis no fundo -->
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

<div class="emoji white-heart1">🤍</div>
<div class="emoji white-heart2">🤍</div>
<div class="emoji white-heart3">🤍</div>
<div class="emoji white-heart4">🤍</div>
<div class="emoji white-heart5">🤍</div>
<div class="emoji white-heart6">🤍</div>
<div class="emoji white-heart7">🤍</div>
<div class="emoji white-heart8">🤍</div>
<div class="emoji white-heart9">🤍</div>
<div class="emoji white-heart10">🤍</div>

</body>
</html>
