# IB-21Generator
<!DOCTYPE html>
<html lang="ru">

<head>
    <meta charset="UTF-8" />
    <title>Генератор случайных цитат</title>
    <style>
        body {
            font-family: Arial, sans-serif;
        }

        #quote-container {
            width: 500px;
            margin: 0 auto;
            padding: 20px;
            border: 1px solid #ccc;
            border-radius: 5px;
            box-shadow: 0 2px 5px #ccc;
        }

        #quote {
            font-size: 1.2rem;
            line-height: 1.5rem;
        }

        #generate-button {
            display: block;
            width: 100%;
            padding: 10px 0;
            margin-top: 20px;
            background-color: #337ab7;
            color: #fff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
    </style>
</head>

<body>
<div id="quote-container">
    <p id="quote"></p>
</div>

<button id="generate-button">Сгенерировать цитату</button>

<script>
    const quotes = [
        "Жизнь слишком коротка, чтобы тратить ее на вещи, которые не приносят радости.",
        "Делай то, что любишь, и ты никогда не будешь работать ни дня в своей жизни.",
        "Если ты не можешь летать, бегай. Если ты не можешь бегать, иди. Если ты не можешь идти, ползи. Но что бы ты ни делал, продолжай двигаться вперед.",
        "Не бойся неудач. Они — ступеньки к успеху.",
        "Лучше жалеть о том, что сделал, чем о том, чего не сделал.",
        "Не жди, пока все станет идеально. Начинай сейчас и делай все возможное.",
        "Не сравнивай себя с другими. Сравнивай себя с тем, кем ты был вчера.",
        "Успех — это не пункт назначения, а путь.",
        "Никогда не сдавайся. Даже когда кажется, что все потеряно.",
        "Вера в себя — первый шаг к успеху.",
    ];

    const quoteElement = document.getElementById("quote");
    const generateButton = document.getElementById("generate-button");

    const generateQuote = () => {
        const randomIndex = Math.floor(Math.random() * quotes.length);
        quoteElement.textContent = quotes[randomIndex];
    };

    generateButton.addEventListener("click", generateQuote);
</script>
</body>

</html>
