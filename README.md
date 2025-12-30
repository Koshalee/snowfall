[snowfall.html](https://github.com/user-attachments/files/24383429/snowfall.html)
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Snowfall</title>
<style>
  body {
    margin: 0;
    overflow: hidden;
    background: transparent;
  }
  .snowflake {
    position: fixed;
    top: -10px;
    color: white;
    font-size: 1em;
    user-select: none;
    animation-name: fall;
    animation-timing-function: linear;
  }
  @keyframes fall {
    to {
      transform: translateY(110vh);
    }
  }
</style>
</head>
<body>

<script>
  const snowflakes = 50;

  for (let i = 0; i < snowflakes; i++) {
    let snow = document.createElement("div");
    snow.className = "snowflake";
    snow.innerHTML = "❄";
    snow.style.left = Math.random() * 100 + "vw";
    snow.style.fontSize = Math.random() * 20 + 10 + "px";
    snow.style.animationDuration = Math.random() * 5 + 5 + "s";
    snow.style.opacity = Math.random();
    document.body.appendChild(snow);
  }
</script>

</body>
</html>
