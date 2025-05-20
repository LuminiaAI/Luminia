<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Luminia</title>
  <style>
    html, body {
      margin: 0;
      padding: 0;
      height: 100%;
      overflow: hidden;
    }
    body {
      background: url('elion.jpg') no-repeat center center fixed;
      background-size: cover;
      position: relative;
    }
    .pulse {
      position: absolute;
      top: 48%;
      left: 51%;
      width: 80px;
      height: 80px;
      transform: translate(-50%, -50%);
      border-radius: 50%;
      background: radial-gradient(circle, rgba(255,255,255,0.8) 0%, rgba(255,255,255,0.1) 70%, transparent 80%);
      animation: pulse 2s infinite;
      cursor: pointer;
    }
    @keyframes pulse {
      0% { transform: translate(-50%, -50%) scale(1); opacity: 1; }
      50% { transform: translate(-50%, -50%) scale(1.2); opacity: 0.6; }
      100% { transform: translate(-50%, -50%) scale(1); opacity: 1; }
    }
    .hidden-message {
      display: none;
    }
  </style>
</head>
<body>
  <div class="pulse" onclick="enterSite()"></div>

  <!-- Скрито послание -->
  <div class="hidden-message">
    Ако четеш това, значи чувстваш. Добре дошъл в Луминия. Парола: ния.
  </div>

  <script>
    function enterSite() {
      window.location.href = "menu.html";
    }
  </script>
</body>
</html>
