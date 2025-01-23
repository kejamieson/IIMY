# IIMY
I'm not as smart as this appears, chatGPT helped. See you soon xx


<html>
<head>
  <title>Is It March Yet?</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      margin-top: 10%;
    }
    .yes {
      color: green;
      font-size: 2em;
    }
    .no {
      color: red;
      font-size: 2em;
    }
    .countdown {
      font-size: 1.2em;
      margin-top: 10px;
    }
 <html>
  <head>
    <style>
      h1 {
        text-align: center;
        color: blueviolet;
      }

      h2 {
        text-align: center;
        border: 1px solid blueviolet;
        padding: 15px;
        border-radius: 10px;
      }

      img {
        width: 100%;
        border-radius: 10px;
      }

      p {
        font-size: 13px;
        line-height: 1.5;
      }

      button {
        width: 100%;
        background: blueviolet;
        border: none;
        padding: 15px;
        box-shadow: 0 15px 20px rgba(0, 0, 0, 0.3);
        border-radius: 30px;
        font-size: 20px;
        color: white;
        margin: 20px 0;
      }

      footer {
        text-align: center;
        font-size: 12px;
      }
    </style>
  </head>
  <body>
    <h1>
      🐧 Penguins
    </h1>
    <h2>
      Birds
    </h2>
    <img
      src="https://c402277.ssl.cf1.rackcdn.com/photos/18435/images/hero_full/Medium_WW267491.jpg?1578425217"
      alt=""
    />
    <p>
      Penguins are flightless seabirds that live almost exclusively below the
      equator. Some island-dwellers can be found in warmer climates, but
      most—including emperor, adélie, chinstrap, and gentoo penguins—reside in
      and around icy Antarctica.
      <br />
      <br />
      <a href="https://en.wikipedia.org/wiki/Penguin">
        Learn more on Wikipedia
      </a>
    </p>
    <button>
      Make a donation
    </button>
    <footer>
      Coded by 👩‍💻
      <a href="https://www.shecodes.io">
        SheCodes
      </a>
    </footer>
    <script>
      function subscribe() {
        let name = prompt("What is your name?");
        prompt("What is your email address?");

        alert(
          `Thanks ${name} for your interest, we'll be in touch! Meanwhile, wash your keyboard 🐧`
        );
      }

      let button = document.querySelector("button");
      button.addEventListener("click", subscribe);
    </script>
  </body>
</html>
      }
    }
  </style>
</head>
<body>
  <h1 id="response"></h1>
  <p id="countdown" class="countdown"></p>
  <img src="https://upload.wikimedia.org/wikipedia/commons/6/67/Cartoon_penguin.png" alt="Penguin Mascot" class="penguin" />

  <script>
    const today = new Date();
    const month = today.getMonth(); // Months are 0-indexed in JavaScript
    const responseElement = document.getElementById("response");
    const countdownElement = document.getElementById("countdown");

    if (month === 2) { // March is month 2 (0 = Jan, 1 = Feb, etc.)
      responseElement.textContent = "Yes, it's March!";
      responseElement.className = "yes";
    } else {
      const nextMarch = new Date(today.getFullYear(), 2, 1);
      if (today.getMonth() > 2) {
        nextMarch.setFullYear(today.getFullYear() + 1);
      }
      const diff = Math.ceil((nextMarch - today) / (1000 * 60 * 60 * 24));
      responseElement.textContent = "No, it's not March yet!";
      responseElement.className = "no";
      countdownElement.textContent = `Only ${diff} day(s) left until March!`;
    }
  </script>
</body>
</html>
