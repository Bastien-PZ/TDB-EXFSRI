# TDB EXFSRI

Ceci est une application [Observable Framework](https://observablehq.com/framework/). Pour installer les dépendances requises, exécutez :

```
npm install
```

Puis pour démarrer le serveur local de visualisation :

```
npm run dev
```

Pour plus d'informations, voir <https://observablehq.com/framework/getting-started>.

## Structure du projet

```ini
.
├─ src
│  ├─ components
│  │  ├─ exctractColumns.js
│  │  ├─ graphHisto.js  
│  │  └─ timeline.js                                
|  | 
│  ├─ data
│  │  ├─ departements.geojson                         # Fichier cartographique pour les départements
│  │  ├─ regions.geojson                              # Fichier cartographique pour les régions
│  │  ├─ recolte_departements_historique.csv          # Fichier de données sur la récolte départementale historique
│  │  ├─ recolte_regions_historique.csv               # Fichier de données sur la récolte régionale historique
│  │  └─ fonctions.js                                 # Fichier de fonctions
|  |           
│  ├─ img
│  │  ├─ img_departements.png                         # Icône des départements
│  │  ├─ img_regions.png                              # Icône des régions
│  │  ├─ img_france.png                               # Icône de la France
│  │  ├─ img_recolte.webp                             # Icône de la récolte
│  │  ├─ img_sciages.webp                             # Icône des sciages
│  │  └─ logo_maasa.png                               # Logo Ministère
|  | 
│  ├─ 1.0.recolte.md                                  # Page d'accueil de la récolte
│  ├─ 1.1.recolte_nationale.md                        # Page de la récolte nationale
│  ├─ 1.2.recolte_regionale.md                        # Page de la récolte régionale
│  ├─ 1.3.recolte_departementale.md                   # Page de la récolte départementale
│  ├─ 2.sciages.md                                    # Page d'accueil des sciages
│  ├─ 3.methodo.md                                    # Page méthodo
│  ├─ 4.pour_en_savoir_plus.md                        # Page pour en savoir plus
│  ├─ 5.a_propos.md                                   # Page à propos
│  ├─ index.md                                        # Page d'accueil de l'app
│  └─ style.css                                       # Page CSS de style
|             
├─ .gitignore
├─ observablehq.config.js    
├─ package.json
└─ README.md
```

## Synthèse des commandes

| Commande           | Description                                              |
| ----------------- | -------------------------------------------------------- |
| `npm install`            | Installer les dépendances                       |
| `npm run dev`        | Démarrer un serveur local de visualisation                             |
| `npm run build`      | Construire le site static en générant `./dist`              |
| `npm run deploy`     | Déployer l'app sur Observable                           |
| `npm run clean`      | Nettoyer le cache local de chargement des données                       |
