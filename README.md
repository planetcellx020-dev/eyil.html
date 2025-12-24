# index.html
hsjsjsh
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>Sembunyi dari EYIL</title>
  <style>
    body {
      background-color: black;
      color: white;
      text-align: center;
      font-family: Arial;
    }
    button {
      padding: 10px 20px;
      margin: 5px;
      font-size: 18px;
    }
  </style>
</head>
<body>

<h1>👁️ SEMBUNYI DARI EYIL 👁️</h1>
<p>Pilih satu pintu untuk bersembunyi</p>

<div id="doors"></div>
<p id="result"></p>

<script>
  let eyilDoor = Math.floor(Math.random() * 5) + 1;

  for (let i = 1; i <= 5; i++) {
    let btn = document.createElement("button");
    btn.innerText = "Pintu " + i;
    btn.onclick = function () {
      if (i === eyilDoor) {
        document.getElementById("result").innerText =
          "❌ EYIL MENEMUKANMU! (Pintu " + eyilDoor + ")";
      } else {
        document.getElementById("result").innerText =
          "✅ KAMU SELAMAT! EYIL ada di pintu " + eyilDoor;
      }
    };
    document.getElementById("doors").appendChild(btn);
  }
</script>

</body>
</html>
