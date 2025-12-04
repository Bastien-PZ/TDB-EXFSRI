---
toc: false
---

<div class="hero">
  <h1>Tableau de bord - Enquête EXF-SRI</h1>
  <h2>Bienvenue sur le site de présentation des résultats de l'enquête Exploitations forestières et sciages (EXF-SRI).</h2>
</div>

<div class="index-container">
  <a href="https://bastien-pz.github.io/TDB-EXFSRI/1.recolte" class="window">
    Récolte de bois<br><br>
    <img src="./img/img_recolte.webp" alt="Récolte de bois" style="width: 500px; height: 150px;">
  </a>
  
  <a href="https://bastien-pz.github.io/TDB-EXFSRI/2.sciages" class="window">
    Production de sciages<br><br>
    <img src="./img/img_sciages.webp" alt="Production de sciages" style="width: 500px; height: 150px;">
  </a>
  
  <a href="https://bastien-pz.github.io/TDB-EXFSRI/3.connexes" class="window">
    Produits connexes<br><br>
  </a>

  <a href="https://bastien-pz.github.io/TDB-EXFSRI/4.methodo" class="window">
    Source et méthodologie
  </a>

  <a href="https://bastien-pz.github.io/TDB-EXFSRI/5.pour_en_savoir_plus" class="window">
    Pour en savoir plus
  </a>

  <a href="https://bastien-pz.github.io/TDB-EXFSRI/6.a_propos" class="window">
    À propos
  </a>
</div>











<style>
  /* Styles pour la grille */
  .index-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
    max-width: 900px;
    margin: auto;
  }

  /* Style pour chaque fenêtre */
  .window {
    background-color: #f0f4f8;
    border: 2px solid #d1d9e6;
    border-radius: 10px;
    text-align: center;
    padding: 20px;
    font-family: Marianne, sans-serif;
    font-size: 20px;
    font-weight: bold;
    color: #333;
    cursor: pointer;
    text-decoration: none;
    transition: transform 0.2s ease, box-shadow 0.2s ease;
  }

  .window:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 15px rgba(0, 0, 0, 0.2);
    background-color: #e6effb;
  }

  .hero {
    display: flex;
    flex-direction: column;
    align-items: center;
    font-family: var(--sans-serif);
    margin: 4rem 0 8rem;
    text-wrap: balance;
    text-align: center;
  }

  .hero h1 {
    margin: 1rem 0;
    padding: 1rem 0;
    max-width: none;
    font-size: 14vw;
    font-weight: 900;
    line-height: 1;
    background: linear-gradient(30deg, var(--theme-foreground-focus), currentColor);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }

  .hero h2 {
    margin: 0;
    max-width: 34em;
    font-size: 20px;
    font-style: initial;
    font-weight: 500;
    line-height: 1.5;
    color: var(--theme-foreground-muted);
  }

  @media (min-width: 640px) {
    .hero h1 {
      font-size: 90px;
    }
  }

</style>
