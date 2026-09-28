---
theme: default
title: SISB — Heure de l'apéro
transition: fade
mdc: true
---

<div class="epfl-header"></div>

<div class="title-slide">

<div class="eyebrow">Heure de l'apéro</div>

# Visualiser les données pour répondre aux bonnes <span class="underline">questions</span>

<div class="subtitle">
De la question à la visualisation : démonstration d’un workflow<br>
Excel → Power Query → Power Pivot | Power BI<br>
en explorant quelques fonctionnalités méconnues des outils Microsoft.
</div>

</div>

---

<div class="epfl-header"></div>

<div class="eyebrow">01 · Introduction</div>

# Voir `[autrement]`

<div class="slide-intro">
Les mêmes données peuvent raconter des histoires très différentes. <br>
Tout dépend de la manière dont on choisit de les présenter.
</div>

<div class="full-visual">

  <img src="/assets/images/01-Extrait-Excel.png">

  <div class="visual-note">
  Deux indicateurs bien réels : les entrées physiques à la Bibliothèque et les prêts physiques.
  </div>

</div>

[Ouvrir le fichier Excel ↗](https://epflch-my.sharepoint.com/:x:/g/personal/genevieve_guex_epfl_ch/IQAaVC0B_0ybQ71Ul3AHfD8vAYURhc2NRJlpyHmimnIRiTE?e=d5V1xL){target="_blank" .demo-link}


---

<div class="epfl-header"></div>

<div class="two-columns">

<div class="left-column">

<div class="eyebrow">01 · Introduction</div>

# Ce que vous voyez

Le graphique donne une forme aux données.<br>
Tendances, écarts et relations deviennent visibles.


</div>

<div class="right-column">

<img src="/assets/images/02-LineChart.gif">

</div>

</div>

---

<div class="epfl-header"></div>

<div class="two-columns">

<div class="left-column">

<div class="eyebrow">01 · Introduction</div>

# Ce que je vois

Les chiffres n’ont pas changé. <br>
Notre manière de les présenter, si.

</div>

<div class="right-column">

<img src="/assets/images/02-Datasaurus.gif">

</div>

</div>

---

<div class="epfl-header"></div>

<div class="two-columns">

<div class="left-column">

<div class="eyebrow">01 · Introduction</div>

# La forme influence le message

<p>
Toute visualisation sélectionne, ordonne et hiérarchise l’information.
</p>

<p class="text-secondary">
Une visualisation structure la perception avant même l’analyse.
</p>

<p v-click="1" class="text-secondary">
Bien choisie, elle éclaire la décision; mal choisie, elle peut la biaiser.
</p>
</div>


<div class="right-column visual-fade">

  <img
    v-click-hide="1"
    class="visual-fade-image"
    src="/assets/images/02-LineChart.png"
    alt="Graphique en courbes"
  />

  <img
    v-click="1"
    class="visual-fade-image"
    src="/assets/images/03-Datasaurus.png"
    alt="Datasaurus"
  />

</div>

</div>