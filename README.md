<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Текст поверх картинки</title>
    <style>
        .image-container {
            position: relative; /* Важно для позиционирования текста */
            display: inline-block; /* Чтобы контейнер был по размеру картинки */
            max-width: 100%;
        }
        .image-container img {
            display: block; /* Убираем лишние отступы */
            width: 100%; /* Адаптивность */
            height: auto;
            border-radius: 10px; /* Опционально: скругление углов */
        }
        .overlay-text {
            position: absolute; /* Позиционируем относительно контейнера */
            top: 50%; /* Центрируем по вертикали */
            left: 50%; /* Центрируем по горизонтали */
            transform: translate(-50%, -50%); /* Точное центрирование */
            color: white; /* Цвет текста */
            font-size: 3rem; /* Размер шрифта */
            font-weight: bold;
            font-family: Arial, sans-serif;
            text-shadow: 
                2px 2px 4px rgba(0, 0, 0, 0.8), /* Тень для читаемости */
                0 0 20px rgba(0, 0, 0, 0.5);
            text-align: center;
            padding: 20px;
            background: rgba(0, 0, 0, 0); /* Полупрозрачный фон для лучшей читаемости */
            border-radius: 10px;
            pointer-events: none; /* Чтобы текст не мешал кликам по картинке */
            width: 80%; /* Ограничиваем ширину текста */
        }

        h2 {
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
            <!-- Замените src на вашу картинку -->
            <img src="https://storage.yandexcloud.net/tsop-cloud-test/for%20email/email_background.png" alt="Пример картинки">
            <div class="overlay-text">
                <h3>451976</h3>
            </div>
        </div>
    </div>
</body>
</html>
