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
        .carousel {
            position: relative;
            width: 100%;
            max-width: 400px;
            margin: 20px auto;
            overflow: hidden;
        }
        .carousel-images {
            display: flex;
            transition: transform 0.5s ease;
        }
        .carousel-images img {
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
            position: relative;
        }
        .carousel-images .text-overlay {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-size: 3rem;
            color: white;
            font-family: 'Pacifico', cursive;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.7);
        }
        .carousel-buttons {
            position: absolute;
            top: 50%;
            width: 100%;
            display: flex;
            justify-content: space-between;
            transform: translateY(-50%);
        }
        .carousel-button {
            background-color: rgba(255, 255, 255, 0.6);
            border: none;
            padding: 10px;
            border-radius: 50%;
            cursor: pointer;
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
        <img src="https://github.com/santoxzs/Amor.html/blob/main/IMG-20241203-WA0007.jpg?raw=true" alt="Imagem do casal">
    </div>

    <div class="carousel">
        <div class="carousel-images" id="carousel-images">
            <div>
                <img src="https://github.com/santoxzs/santoxzs.github.io/blob/main/IMG-20250128-WA0023.jpg?raw=true" alt="Imagem 1">
                <div class="text-overlay">Eu</div>
            </div>
            <div>
                <img src="https://github.com/santoxzs/Minha-quian-a-/blob/main/IMG_20241203_115037_136.jpg?raw=true" alt="Imagem 2">
                <div class="text-overlay">Te</div>
