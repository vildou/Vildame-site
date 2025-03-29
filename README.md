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

