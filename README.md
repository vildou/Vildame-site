
!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Vild’âme - Guidance du jour</title>
  <style>
    body {
      font-family: 'Georgia', serif;
      background-color: #fffaf7;
      color: #3b2f2f;
      margin: 0;
      padding: 2rem;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 2rem;
    }

    img.logo {
      width: 250px;
      border-radius: 16px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    }

    .section {
      text-align: center;
      max-width: 90%;
    }

    .section-title {
      font-weight: bold;
      margin-bottom: 0.5rem;
      text-transform: uppercase;
      letter-spacing: 1px;
      font-size: 1rem;
      color: #b89c7d;
    }

    .carte {
      border: 2px dashed #e2d5c3;
      border-radius: 16px;
      padding: 1.5rem;
      background-color: #fdfaf7;
      font-style: italic;
      font-size: 1.3rem;
      text-align: center;
      min-height: 80px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.05);
      margin-top: 0.5rem;
    }

    .paypal {
      margin-top: 2rem;
    }

    .paypal a {
      background-color: #d4bfa3;
      color: white;
      padding: 0.8rem 1.5rem;
      border-radius: 8px;
      text-decoration: none;
      font-weight: bold;
    }
  </style>
</head>
<body>

  <!-- Logo -->
  <img src="https://raw.githubusercontent.com/vildou/Vildame-site/main/logo-vildame.jpg" alt="Logo Vild'âme" class="logo" />

  <!-- Carte du jour -->
  <div class="section">
    <div class="section-title">Carte du jour</div>
    <div class="carte" id="carte-jour">Tirage en cours...</div>
  </div>

  <!-- Carte de guérison -->
  <div class="section">
    <div class="section-title">Carte de guérison</div>
    <div class="carte" id="carte-guerison">Tirage en cours...</div>
  </div>

  <!-- Carte de guidance -->
  <div class="section">
    <div class="section-title">Carte de guidance</div>
    <div class="carte" id="carte-guidance">Tirage en cours...</div>
  </div>

  <!-- PayPal -->
  <div class="paypal">
    <p>Tu veux soutenir Vild’âme ?</p>
    <a href="https://www.paypal.com/donate/?hosted_button_id=XXXXXXXXXXX" target="_blank">Faire un don</a>
  </div>

  <script>
    const cartesJour = [
      "Aujourd’hui, je me choisis avec douceur.",
      "Respire. Tu es exactement là où tu dois être.",
      "Je suis en sécurité, ancrée et alignée.",
      "Je mérite l’amour, la lumière et l’abondance.",
      "Je laisse le passé derrière et j’avance en confiance."
    ];

    const cartesGuerison = [
      "Mon souffle m’apaise et me régénère.",
      "Chaque cellule de mon corps reçoit de la lumière.",
      "Je m’autorise à guérir à mon rythme.",
      "La paix est mon refuge intérieur.",
      "Je libère ce qui ne m’appartient plus."
    ];

    const cartesGuidance = [
      "La bonne clé est celle qui vibre en toi.",
      "Ton intuition connaît déjà le chemin.",
      "Accueille ce qui vient avec foi.",
      "L’univers conspire en ta faveur.",
      "Avance avec confiance, chaque pas est guidé."
    ];

    function tirerCarte(id, cartes) {
      const zone = document.getElementById(id);
      setTimeout(() => {
        const tirage = cartes[Math.floor(Math.random() * cartes.length)];
        zone.innerText = tirage;
      }, 2000); // animation de tirage
    }

    tirerCarte("carte-jour", cartesJour);
    tirerCarte("carte-guerison", cartesGuerison);
    tirerCarte("carte-guidance", cartesGuidance);
  </script>

</body>
</html>
