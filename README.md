# Floresss
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Campo de Flores Amarillas</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: flex-end;
            height: 100vh;
            background: linear-gradient(to top, #88d498, #87CEEB);
            overflow: hidden;
            position: relative;
        }

        .campo {
            display: flex;
            justify-content: center;
            align-items: flex-end;
            width: 100%;
            height: 100%;
            position: absolute;
            bottom: 0;
        }

        .flor {
            position: relative;
            width: 120px;
            height: 120px;
            margin: 0 20px;
            animation: viento 4s infinite ease-in-out alternate;
        }

        .flor:nth-child(even) {
            animation-duration: 5s;
        }

        .petalo {
            position: absolute;
            width: 55px;
            height: 90px;
            background: radial-gradient(circle, #ffd700, #ffcc00);
            border-radius: 60% 80% 70% 90%;
            top: 15px;
            left: 32px;
            transform-origin: 50% 80%;
            animation: moverPetalo 2s infinite ease-in-out alternate;
        }

        .flor .petalo:nth-child(1) { transform: rotate(0deg); animation-delay: 0.2s; }
        .flor .petalo:nth-child(2) { transform: rotate(45deg); animation-delay: 0.4s; }
        .flor .petalo:nth-child(3) { transform: rotate(90deg); animation-delay: 0.6s; }
        .flor .petalo:nth-child(4) { transform: rotate(135deg); animation-delay: 0.8s; }
        .flor .petalo:nth-child(5) { transform: rotate(180deg); animation-delay: 1s; }
        .flor .petalo:nth-child(6) { transform: rotate(225deg); animation-delay: 1.2s; }
        .flor .petalo:nth-child(7) { transform: rotate(270deg); animation-delay: 1.4s; }
        .flor .petalo:nth-child(8) { transform: rotate(315deg); animation-delay: 1.6s; }

        .centro {
            position: absolute;
            width: 50px;
            height: 50px;
            background: radial-gradient(circle, #ff8c00, #cc7700);
            border-radius: 50%;
            top: 35px;
            left: 35px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
        }

        .tallo {
            position: absolute;
            width: 15px;
            height: 170px;
            background: linear-gradient(to bottom, #3aaf3a, #2a8f2a);
            top: 100px;
            left: 53px;
            border-radius: 10px;
            animation: moverTallo 4s infinite ease-in-out alternate;
        }

        .hoja {
            position: absolute;
            width: 50px;
            height: 25px;
            background: linear-gradient(to right, #3aaf3a, #2a8f2a);
            border-radius: 50%;
            top: 120px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
        }

        .hoja.izquierda {
            left: 10px;
            transform: rotate(-30deg);
            animation: moverHoja 3s infinite ease-in-out alternate;
        }

        .hoja.derecha {
            left: 55px;
            transform: rotate(30deg);
            animation: moverHoja 3s infinite ease-in-out alternate-reverse;
        }

        /* Animaciones */
        @keyframes moverPetalo {
            0% { transform: scale(1); }
            100% { transform: scale(1.1); }
        }

        @keyframes viento {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(3deg); }
        }

        @keyframes moverTallo {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(2deg); }
        }

        @keyframes moverHoja {
            0% { transform: rotate(-30deg) scale(1); }
            100% { transform: rotate(-35deg) scale(1.1); }
        }
    </style>
</head>
<body>
    <div class="campo">
        <div class="flor">
            <div class="petalo"></div>
            <div class="petalo"></div>
            <div class="petalo"></div>
            <div class="petalo"></div>
            <div class="petalo"></div>
            <div class="petalo"></div>
            <div class="petalo"></div>
            <div class="petalo"></div>
            <div class="centro"></div>
            <div class="tallo"></div>
            <div class="hoja izquierda"></div>
            <div class="hoja derecha"></div>
        </div>

        <div class="flor">
            <div class="petalo"></div>
            <div class="petalo"></div>
            <div class="petalo"></div>
            <div class="petalo"></div>
            <div class="petalo"></div>
            <div class="petalo"></div>
            <div class="petalo"></div>
            <div class="petalo"></div>
            <div class="centro"></div>
            <div class="tallo"></div>
            <div class="hoja izquierda"></div>
            <div class="hoja derecha"></div>
        </div>

        <div class="flor">
            <div class="petalo"></div>
            <div class="petalo"></div>
            <div class="petalo"></div>
            <div class="petalo"></div>
            <div class="petalo"></div>
            <div class="petalo"></div>
            <div class="petalo"></div>
            <div class="petalo"></div>
            <div class="centro"></div>
            <div class="tallo"></div>
            <div class="hoja izquierda"></div>
            <div class="hoja derecha"></div>
        </div>
    </div>
</body>
</html>

