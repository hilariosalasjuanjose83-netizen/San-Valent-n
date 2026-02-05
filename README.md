<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>San Valentín 💘</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #ffe6eb;
      text-align: center;
      padding-top: 100px;
    }
    h1 {
      font-size: 2.5em;
      color: #d6336c;
    }
    button {
      font-size: 1.2em;
      padding: 15px 30px;
      margin: 20px;
      border: none;
      border-radius: 10px;
      cursor: pointer;
    }
    #si {
      background-color: #ff4d6d;
      color: white;
    }
    #no {
      background-color: #adb5bd;
      position: absolute;
    }
  </style>
</head>
<body>

  <h1>¿Quieres ser mi San Valentín? 💖</h1>

  <button id="si" onclick="aceptar()">Sí</button>
  <button id="no" onmouseover="moverNo()">No</button>

  <script>
    function aceptar() {
      document.body.innerHTML = "<h1>💘 Sabía que dirías que sí 💘</h1>";
    }

    function moverNo() {
      const x = Math.random() * (window.innerWidth - 100);
      const y = Math.random() * (window.innerHeight - 50);
      const noBtn = document.getElementById("no");
      noBtn.style.left = x + "px";
      noBtn.style.top = y + "px";
    }
  </script>

</body>
</html>
