<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Текст поверх картинки</title>
    <style>
        .image-container {
            position: relative;
            display: inline-block; 
            max-width: 100%;
        }
        .image-container img {
            display: block; 
            width: 100%; 
            height: auto;
            border-radius: 10px;
        }
        .overlay-text {
            position: absolute; 
            top: 50%; 
            left: 50%;
            transform: translate(-50%, -50%);
            color: white;
            font-size: 3rem; 
            font-weight: bold;
            font-family: Arial, sans-serif;
            text-shadow: 
                2px 2px 4px rgba(0, 0, 0, 0.8),
                0 0 20px rgba(0, 0, 0, 0.5);
            text-align: center;
            padding: 20px;
            background: rgba(0, 0, 0, 0);
            border-radius: 10px;
            pointer-events: none; 
            width: 80%; 
        }
        .h2 {
            color: white;
            margin: 0;
        }
        .example {
            text-align: center;
        }
        .example p {
            color: #aaa;
            margin-top: 10px;
        }
    </style>
</head>
<body>
    <div class="example">
        <div class="image-container">
            <img src="https://storage.yandexcloud.net/tsop-cloud-test/for%20email/email_background.png" alt="Пример картинки">
            <div class="overlay-text">
                <h3>451976</h3>
            </div>
        </div>
    </div>
</body>
</html>
