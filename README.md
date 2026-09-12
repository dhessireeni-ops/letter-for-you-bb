<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>A Letter For You</title>

    <style>
        body {
            margin: 0;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            background: #f6e9e9;
            font-family: Georgia, serif;
            padding: 30px 0;
            box-sizing: border-box;
        }

        /* YouTube video */
        .music {
            text-align: center;
            margin-bottom: 40px;
        }

        .music p {
            margin-bottom: 10px;
            font-size: 18px;
        }

        .music iframe {
            width: 280px;
            height: 80px;
            border: none;
        }

        /* Envelope and letter container */
        .container {
            text-align: center;
            width: 100%;
        }

        /* Envelope */
        .envelope {
            width: 300px;
            height: 200px;
            background: #d99a9a;
            position: relative;
            margin: 0 auto;
            cursor: pointer;
            border-radius: 5px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.2);
        }

        .flap {
            position: absolute;
            top: 0;
            left: 0;
            width: 0;
            height: 0;
            border-left: 150px solid transparent;
            border-right: 150px solid transparent;
            border-top: 100px solid #c77f7f;
            transition: 0.6s;
            transform-origin: top;
            z-index: 2;
        }

        .heart {
            position: absolute;
            top: 75px;
            left: 125px;
            font-size: 45px;
            z-index: 3;
        }

        /* Letter */
        .letter {
            display: none;
            background: white;
            width: 320px;
            max-width: 85%;
            padding: 30px;
            margin: 20px auto;
            border-radius: 10px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            animation: appear 0.8s ease;
            box-sizing: border-box;
        }

        .letter h1 {
            color: #a84c4c;
        }

        .letter p {
            color: #444;
            line-height: 1.7;
            text-align: left;
            white-space: pre-line;
        }

        button {
            background: #a84c4c;
            color: white;
            border: none;
            padding: 12px 20px;
            border-radius: 20px;
            cursor: pointer;
            font-size: 15px;
        }

        button:hover {
            background: #843737;
        }

        #hiddenMessage {
            display: none;
            margin-top: 20px;
            color: #a84c4c;
            font-style: italic;
        }

        @keyframes appear {
            from {
                opacity: 0;
                transform: translateY(30px);
            }

            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
</head>

<body>

    <!-- YOUTUBE VIDEO -->
    <div class="music">

        <p>Our theme song.</p>

       <video autoplay muted loop controls width="300" height="200">
    <source src="allineedtohear.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>

    </div>


    <!-- ENVELOPE AND LETTER -->
    <div class="container">
        <div class="envelope" id="envelope" onclick="openLetter()">
            <div class="flap"></div>
            <div class="heart">♡</div>
        </div>

        <p id="instruction">Click here babyy.</p>


        <!-- LETTER -->
        <div class="letter" id="letter">

            <h1>For You</h1>

            <p>
Dear xis, my baby^^<3

i wanted to make something special for you,
so instead of sending an ordinary message hihi,
i made you this little letter for our first monthsaryTvT

happy monthsary, my baby! ♡

another month with you, and somehow you still haven’t gotten tired of me noh grabi kaya kita idol eh, i’m honestly impressed baby. either your patience is incredible, or you have questionable decision-making skills that you've decided to stay. either way, i’m keeping you.

i want you to know how much i love having you in my life like really. you’ve become someone i look forward to talking to, someone i feel comfortable with, and someone who makes even the most ordinary days feel a little more special. my whole family knows you already and i won't make a reckless decision by making a small conflict tear us apart.

i love our silly conversations, our random moments, our teasing, and even the little things we do that probably make absolutely no sense sa uban huhu. i love being able to be myself around you, whether i’m being sweet, annoying, dramatic, clingy, or all emotions at once char, sadness lumabas ka.

thank you for being patient with me. thank you for listening to my random stories, respecting my boundaries, and making me feel heard and appreciated. i notice those things, even when i don’t always say it.

i hope you know i’m not here because everything is perfect. i’m here because i genuinely like you, i care about you, and i want to keep choosing you as we continue learning more about each other.

so, happy monthsary to us. another month of love, laughter, questionable decisions, random conversations, and me stealing your attention whenever i feel like it.

i love you, silly. please remain my silly for a long time MWAAAAAA. ♡

yours,
dhes cute sobra
            </p>

            <hr>

            <p>
thank you for being someone who makes ordinary
moments feel meaningful kanya kanya na to baby, pero akin ka okay i love youy
            </p>

            <p>
with love,<br>
dhessireeeerer
            </p>

            <button onclick="showMessage()">
                last thing...
            </button>

            <p id="hiddenMessage">
                no words can explain how much i adore you, alexis. you made me happy in a way i never thought i could feel. my life had always been mudane, but when you came it changed—not drastically but slowly that it felt like home.
            </p>

        </div>

    </div>


    <script>

        function openLetter() {

            document.getElementById("envelope").style.display = "none";

            document.getElementById("instruction").style.display = "none";

            document.getElementById("letter").style.display = "block";

        }


        function showMessage() {

            document.getElementById("hiddenMessage").style.display = "block";

        }

    </script>

</body>
</html>
