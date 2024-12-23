<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Permohonan Maaf</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(120deg, #f6d365 0%, #fda085 100%);
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .container {
            background-color: #ffffff;
            padding: 30px;
            box-shadow: 0 15px 25px rgba(0, 0, 0, 0.1);
            text-align: center;
            border-radius: 10px;
            transition: transform 0.3s;
        }
        .container:hover {
            transform: scale(1.05);
        }
        h1 {
            color: #444;
            margin-bottom: 20px;
        }
        p {
            color: #666;
            line-height: 1.6;
            margin-bottom: 20px;
        }
        .buttons {
            margin-top: 20px;
        }
        .buttons button {
            padding: 12px 25px;
            margin: 5px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s, transform 0.3s;
        }
        .forgive {
            background-color: #28a745;
            color: white;
        }
        .forgive:hover {
            background-color: #218838;
            transform: scale(1.05);
        }
        .not-forgive {
            background-color: #dc3545;
            color: white;
            position: relative;
        }
        .not-forgive:hover {
            background-color: #c82333;
            transform: scale(1.05);
        }
        .signature {
            margin-top: 20px;
            font-style: italic;
            color: #777;
        }
    </style>
    <script>
        function moveButton() {
            const button = document.querySelector('.not-forgive');
            const x = Math.random() * (window.innerWidth - button.offsetWidth);
            const y = Math.random() * (window.innerHeight - button.offsetHeight);
            button.style.position = 'absolute';
            button.style.left = x + 'px';
            button.style.top = y + 'px';
        }
    </script>
</head>
<body>
    <div class="container">
        <h1>Permohonan Maaf</h1>
        <p>Dear [among],</p>
        <p>Saya ingin meminta maaf atas kesalahan yang telah saya lakukan.</p>
        <div class="buttons">
            <button class="forgive" onclick="alert('Anda telah dimaafkan!')">Maafkan</button>
            <button class="not-forgive" onclick="moveButton()">Tidak Maafkan</button>
        </div>
        <div class="signature">
            Dengan hormat,<br>[ukki]
        </div>
    </div>
</body>
</html>
