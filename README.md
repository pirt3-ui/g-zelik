# g-zelik
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Barış Teklifi</title>
    <style>
        body {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #fce4ec;
            font-family: Arial, sans-serif;
            text-align: center;
            overflow: hidden;
            margin: 0;
        }
        img {
            width: 300px;
            height: auto;
            border-radius: 10px;
        }
        h2 {
            margin: 20px 0;
        }
        .buttons {
            display: flex;
            gap: 20px;
            position: relative;
        }
        button {
            padding: 10px 20px;
            font-size: 18px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }
        .yes {
            background-color: #4CAF50;
            color: white;
            margin-left: 100px;
        }
        .no {
            background-color: #e74c3c;
            color: white;
            position: absolute;
            transition: transform 0.2s ease;
        }
    </style>
</head>
<body>
    <img src="f232992ea97dbd6d147f7f64e2486d51.jpg" alt="Barış Teklifi">
    <h2>Seni Üzdüğüm İçin Özür Dilerim, Barışalımmı Güzelimm?</h2>
    <div class="buttons">
        <button class="yes" onclick="window.location.href='teskur.html'">Evet</button>
        <button class="no" id="noButton">Hayır</button>
    </div>

    <script>
        const noButton = document.getElementById("noButton");

        function moveButton() {
            const maxX = window.innerWidth - 100;
            const maxY = window.innerHeight - 100;
            const x = Math.random() * maxX;
            const y = Math.random() * maxY;
            noButton.style.transform = `translate(${x}px, ${y}px)`;
        }

        noButton.addEventListener("mouseover", moveButton);
        noButton.addEventListener("touchstart", moveButton); // Dokunmatik cihazlarda çalışması için
    </script>
</body>
</html>
