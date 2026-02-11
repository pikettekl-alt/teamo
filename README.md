# teamo
jiji
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>🥺</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #ffe6f0;
      height: 100vh;
      margin: 0;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .box {
      background: white;
      padding: 30px;
      border-radius: 15px;
      text-align: center;
      box-shadow: 0 10px 20px rgba(0,0,0,0.2);
      position: relative;
      width: 300px;
    }

    button {
      padding: 10px 20px;
      font-size: 16px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      margin: 10px;
    }

    #si {
      background-color: #ff4d88;
      color: white;
    }

    #no {
      background-color: #ccc;
      position: absolute;
    }
  </style>
</head>
<body>

  <div class="box">
    <h1>ola ti amu 🥺</h1>
    <p>mi amas?</p>
    <button id="si" onclick="alert('sabía 😳💖')">sí</button>
    <button id="no">no</button>
  </div>

  <script>
    const noBtn = document.getElementById("no");
    const box = document.querySelector(".box");

    noBtn.addEventListener("mouseover", () => {
      const maxX = box.clientWidth - noBtn.offsetWidth;
      const maxY = box.clientHeight - noBtn.offsetHeight;

      const x = Math.random() * maxX;
      const y = Math.random() * maxY;

      noBtn.style.left = x + "px";
      noBtn.style.top = y + "px";
    });
  </script>

</body>
</html>
