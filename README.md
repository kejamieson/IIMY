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
    <title>Estonian Flag Snowfall</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="snow-container"></div>
    <script src="script.js"></script>
</body>
</html>
