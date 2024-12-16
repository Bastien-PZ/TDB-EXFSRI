---
toc: false
---

<div class="hero">
  <h1>TDB EXFSRI</h1>
  <h2>Welcome to your new app! Edit&nbsp;<code style="font-size: 90%;">src/index.md</code> to change this page.</h2>
  <a href="https://observablehq.com/framework/getting-started">Get started<span style="display: inline-block; margin-left: 0.25rem;">↗︎</span></a>
</div>

<div class="grid grid-cols-2" style="grid-auto-rows: 504px;">
  <div class="card">${
    resize((width) => Plot.plot({
      title: "Your awesomeness over time 🚀",
      subtitle: "Up and to the right!",
      width,
      y: {grid: true, label: "Awesomeness"},
      marks: [
        Plot.ruleY([0]),
        Plot.lineY(aapl, {x: "Date", y: "Close", tip: true})
      ]
    }))
  }</div>
  <div class="card">${
    resize((width) => Plot.plot({
      title: "How big are penguins, anyway? 🐧",
      width,
      grid: true,
      x: {label: "Body mass (g)"},
      y: {label: "Flipper length (mm)"},
      color: {legend: true},
      marks: [
        Plot.linearRegressionY(penguins, {x: "body_mass_g", y: "flipper_length_mm", stroke: "species"}),
        Plot.dot(penguins, {x: "body_mass_g", y: "flipper_length_mm", stroke: "species", tip: true})
      ]
    }))
  }</div>
</div>

---

html`
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
    font-family: Arial, sans-serif;
    font-size: 16px;
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
</style>

<div class="index-container">
  <!-- Fenêtre 1 -->
  <a href="https://bastien-pz.github.io/TDB-EXFSRI/recolte" class="window">
    Page 1 : Introduction
  </a>
  
  <!-- Fenêtre 2 -->
  <a href="https://observablehq.com/@utilisateur/page2" class="window">
    Page 2 : Analyse des données
  </a>
  
  <!-- Fenêtre 3 -->
  <a href="https://observablehq.com/@utilisateur/page3" class="window">
    Page 3 : Visualisations
  </a>
  
  <!-- Fenêtre 4 -->
  <a href="https://observablehq.com/@utilisateur/page4" class="window">
    Page 4 : Tableau de bord
  </a>
  
  <!-- Fenêtre 5 -->
  <a href="https://observablehq.com/@utilisateur/page5" class="window">
    Page 5 : Interactions
  </a>
  
  <!-- Fenêtre 6 -->
  <a href="https://observablehq.com/@utilisateur/page6" class="window">
    Page 6 : Conclusion
  </a>
</div>
`


<style>

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
