# Convite
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <title>Convite Especial</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #ffeaea;
      text-align: center;
      padding-top: 100px;
    }

    h1 {
      color: #ff4d6d;
      font-size: 2em;
    }

    .btn {
      padding: 10px 20px;
      margin: 20px;
      font-size: 1em;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      transition: 0.3s;
    }

    #yesBtn {
      background-color: #ffb6b9;
      color: white;
    }

    #noBtn {
      background-color: #ccc;
      color: black;
      position: absolute;
    }

    #response {
      font-size: 1.5em;
      color: #ff4d6d;
      margin-top: 30px;
    }
  </style>
</head>
<body>
  <h1>Você aceita ir ao cinema comigo?</h1>

  <button id="yesBtn" class="btn">Sim</button>
  <button id="noBtn" class="btn">Não</button>

  <div id="response"></div>

  <script>
    const yesBtn = document.getElementById("yesBtn");
    const noBtn = document.getElementById("noBtn");
    const response = document.getElementById("response");

    yesBtn.onclick = () => {
      response.innerHTML = "Oba! Mal posso esperar!";
    };

    noBtn.onmouseover = () => {
      const x = Math.random() * (window.innerWidth - 100);
      const y = Math.random() * (window.innerHeight - 50);
      noBtn.style.left = x + "px";
      noBtn.style.top = y + "px";
    };
  </script>
</body>
</html>
