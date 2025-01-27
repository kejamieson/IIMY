# IIMY
I'm not as smart as this appears, despite my myspace era - chatGPT helped xx


<html>
<head>
  <title>Is It March Yet?</title>
  <style>
    body { font-family: Monotype Corsiva, sans-serif; text-align: center; margin-top: 20%; }
    .yes { color: green; font-size: 2em; }
    .no { color: red; font-size: 2em; }
    .countdown { font-size: 1.2em; margin-top: 10px; }
  </style>
</head>
<body>
  <h1 id="response"></h1>
  <p id="countdown" class="countdown"></p>
  <script>
    const today = new Date();
    const month = today.getMonth(); // Months are 0-indexed in JavaScript
    const responseElement = document.getElementById("response");
    const countdownElement = document.getElementById("countdown");

    if (month === 2) { // March is month 2 (0 = Jan, 1 = Feb, etc.)
      responseElement.textContent = "Yes, it's March! See you soon? :) ";
      responseElement.className = "yes";
    } else {
      const nextMarch = new Date(today.getFullYear(), 2, 1);
      if (today.getMonth() > 2) {
        nextMarch.setFullYear(today.getFullYear() + 1);
      }
      const diff = Math.ceil((nextMarch - today) / (1000 * 60 * 60 * 24));
      responseElement.textContent = "Not Yet...";
      responseElement.className = "no";
      countdownElement.textContent = `Only ${diff} day(s) left until March!`;
    }
  </script>
</body>

<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Estonian Flag Spiral Effect</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      background-color: #f0f0f0;
      display: flex;
      justify-content: center;
      align-items: center;
      overflow: hidden;
      background-color: black;
    }

    #flag {
      width: 300px;
      height: 200px;
      position: absolute;
      transform-origin: center;
      animation: spiral 5s ease-out forwards, disappear 1s 5s forwards;
    }

    .stripe {
      width: 100%;
      height: 33.33%;
    }

    .blue {
      background-color: #0072CE;
    }

    .black {
      background-color: #FFFFFF;
    }

    .white {
      background-color: #FFFFFF;
    }

    @keyframes spiral {
      0% {
        transform: scale(1) rotate(0deg);
        opacity: 1;
      }
      100% {
        transform: scale(0) rotate(1440deg);
        opacity: 0;
      }
    }

    @keyframes disappear {
      0% {
        opacity: 1;
      }
      100% {
        opacity: 0;
      }
    }
  </style>
</head>
<body>

  <div id="flag">
    <div class="stripe blue"></div>
    <div class="stripe black"></div>
    <div class="stripe white"></div>
  </div>

</body>
</html>

