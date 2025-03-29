<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Vild'âme</title>
  <style>
    div id="carte-du-jour" style="margin-top: 2rem; padding: 1.5rem; border: 2px dashed #e2d5c3; border-radius: 16px; background-color: #fdfaf7; font-style: italic; font-size: 1.2rem; text-align: center;"></div>

<script>
  const cartes = [
    "Aujourd’hui, je me choisis avec douceur.",
    "Respire. Tu es exactement là où tu dois être.",
    "La bonne clé est celle qui vibre en toi.",
    "Je suis en sécurité, ancrée et alignée.",
    "Chaque souffle m’ouvre un peu plus à la paix.",
    "Mon intuition me guide avec sagesse.",
    "Je mérite l’amour, la lumière et l’abondance.",
    "Je suis reliée à la beauté de la vie.",
    "Je laisse le passé derrière et j’avance en confiance."
  ];

  const carte = cartes[Math.floor(Math.random() * cartes.length)];
  document.getElementById("carte-du-jour").innerText = carte;
</script>


    body {
      margin: 0;
      padding: 0;
      background: #fdf9f3;
      font-family: 'Georgia', serif;
      color: #5a4a3f;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      text-align: center;
    }
    .container {
      max-width: 600px;
      padding: 2rem;
      border: 2px solid #e2d5c3;
      border-radius: 12px;
      background: #fffaf5;
      box-shadow: 0 0 10px rgba(0,0,0,0.05);
    }
    h1 {
      font-size: 2rem;
      margin-bottom: 1.5rem;
    }
    p {
      font-size: 1.1rem;
      line-height: 1.6;
    }
    .signature {
      margin-top: 2rem;
      font-style: italic;
    }
    .button {
      margin-top: 2rem;
      display: inline-block;
      padding: 0.8rem 1.5rem;
      background: #d2b48c;
      color: white;
      text-decoration: none;
      border-radius: 8px;
      font-weight: bold;
    }
    .button:hover {
      background: #b6966c;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Bienvenue dans l'univers Vild'âme</h1>
    <p>Ici, chaque souffle,<br>
    chaque mot, chaque rituel<br>
    est une clé vers ton monde intérieur.</p>

    <p>Prends ce temps pour toi,<br>
    pour t'écouter, pour t'honorer.</p>

    <p><strong>Vild'âme te murmure :</strong><br>
    "La bonne clé est celle qui vibre en toi."</p>

    <div class="signature">– Vildou</div>

    <a href="#" class="button">Entrer dans l'univers</a>
  </div>
</body>
</html>
