---
toc: false
comments: false
layout: post
title: Bonk the Teemo
description: Hit this annoying little scoundrel 
type: tangibles
courses: { compsci: {week: 3} }
---


![teemoannoying]({{ site.baseurl }}/images/annoyingteemo.jpeg)


<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Bonk the Teemo</title>
    <style>
        #bonk-button {
            background-color: #2196F3;
            color: #fff;
            padding: 10px 20px;
            font-size: 18px;
            border: none;
            cursor: pointer;
        }
        #bonk-counter {
            font-size: 24px;
            margin-top: 20px;
        }
        #random-text {
            font-size: 18px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <button id="bonk-button">Bonk Teemo</button>
    <div id="bonk-counter">Bonk Count: 0</div>
    <div id="random-text">Text: </div>

    <script>
        const bonkButton = document.getElementById('bonk-button');
        const bonkCounter = document.getElementById('bonk-counter');
        const randomText = document.getElementById('random-text');
        let count = 0;

        bonkButton.addEventListener('click', () => {
            count++;
            bonkCounter.textContent = `Bonk Count: ${count}`;

            const randomNum = Math.random();
            let textToShow = '';

            if (randomNum < 0.01) {
                textToShow = 'The Twelfth day Where the Black sun Dies will Engulf the World in Flames.';
            } else {
                const randomTexts = ['ow!', 'no sir!'];
                textToShow = randomTexts[Math.floor(Math.random() * randomTexts.length)];
            }

            randomText.textContent = `Text: ${textToShow}`;
        });
    </script>
</body>
</html>
