<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <title>Roue de la Fortune</title>
    <style>
        .wheel-container {
            position: relative;
            width: 300px;
            height: 300px;
            margin: 50px auto;
        }
        .wheel {
            width: 100%;
            height: 100%;
            border-radius: 50%;
            border: 5px solid #333;
            transition: transform 4s cubic-bezier(0.17, 0.67, 0.1, 1);
        }
        .pointer {
            position: absolute;
            top: -20px;
            left: 50%;
            transform: translateX(-50%);
            width: 0;
            height: 0;
            border-left: 15px solid transparent;
            border-right: 15px solid transparent;
            border-top: 30px solid red;
            z-index: 10;
        }
        button {
            display: block;
            margin: 20px auto;
            padding: 10px 20px;
            font-size: 16px;
        }
    </style>
</head>
<body>

<div class="wheel-container">
    <div class="pointer"></div>
    <img src="votre-image-de-roue.png" id="wheel" class="wheel" alt="Roue">
</div>

<button onclick="spinWheel()">Tourner la roue</button>

<script>
    let currentRotation = 0;

    function spinWheel() {
        // Génère une rotation aléatoire d'au moins 5 tours complets + un angle aléatoire
        const extraDegrees = Math.floor(Math.random() * 360);
        currentRotation += 1800 + extraDegrees; 
        
        document.getElementById('wheel').style.transform = `rotate(${currentRotation}deg)`;
    }
</script>

</body>
</html>
