---
theme: default
title: SISB — Heure de l'apéro
transition: fade
mdc: true
hideInToc: true
---

<div class="title-slide">

<div class="eyebrow">Heure de l'apéro</div>

# Visualiser les données pour répondre aux bonnes <span class="underline">questions</span>

<div class="subtitle">
De la question à la visualisation : démonstration d’un workflow<br>
<strong>Excel → Power Query → Power Pivot | Power BI</strong><br>
en explorant quelques fonctionnalités méconnues des outils Microsoft.
</div>

</div>

---
hideInToc: true
---

<div class="eyebrow">Sommaire</div>

# Aujourd’hui

<Toc minDepth="1" maxDepth="1" />

---
title: 01 · Introduction · partir d’une question
level: 1
---

<div class="eyebrow">01 · Introduction</div>

# Voir `[autrement]`

<div class="slide-intro">
Les données brutes décrivent une réalité, mais elles ne la rendent pas immédiatement visible.
</div>

<div class="full-visual">
  <img src="/assets/images/01-01-Extrait-Excel.png">
</div>

[Ouvrir le fichier Excel ↗](https://epflch-my.sharepoint.com/:x:/g/personal/genevieve_guex_epfl_ch/IQAaVC0B_0ybQ71Ul3AHfD8vAYURhc2NRJlpyHmimnIRiTE?e=d5V1xL){target="_blank" .demo-link}

<p class="text-secondary">
Face au tableau, notre cerveau doit lire, mémoriser et comparer une succession de nombres.
</p>

---
hideInToc: true
---

<div class="two-columns">

<div class="left-column">

<div class="eyebrow">01 · Introduction</div>

# Ce que vous voyez

<div class="slide-intro">
La visualisation transforme des valeurs en formes, écarts et relations que nous pouvons comparer.
</div>

<p class="text-secondary">
Le graphique donne une forme aux données.<br>
Tendances, écarts et relations deviennent visibles.
</p>

</div>

<div class="right-column">
  <img src="/assets/images/01-02-LineChart.gif">
</div>

</div>

---
hideInToc: true
---

<div class="two-columns">

<div class="left-column">

<div class="eyebrow">01 · Introduction</div>

# Ce que vous ne voyez pas

<div class="slide-intro">
Les chiffres n’ont pas changé. <br>
La question que nous leur posons a changé.
</div>

<p class="text-secondary">
Une autre question fait apparaître une autre structure dans les mêmes données.
</p>

</div>

<div class="right-column">
  <img src="/assets/images/01-03-Datasaurus.gif">
</div>

</div>

---
hideInToc: true
---

<div class="two-columns">

<div class="left-column">

<div class="eyebrow">01 · Introduction</div>

# Changer de point de vue

<div class="slide-intro">
Une seule vue suffit rarement.
</div>

<p class="text-secondary">
Comparer, vérifier et changer de perspective permet de mieux comprendre les données.
</p>

<p v-click="1" class="text-secondary">
Avant de conclure, il faut vérifier ce que l’on voit - et ce que l’on ne voit pas.
</p>

</div>

<div class="right-column visual-fade">
  <img
    v-click-hide="1"
    class="visual-fade-image"
    src="/assets/images/01-04-LineChart.png"
    alt="Graphique en courbes"
  />

  <img
    v-click="1"
    class="visual-fade-image"
    src="/assets/images/03-Datasaurus.png"
    alt="Datasaurus"
  />
</div>

<div class="source-note">
Original Datasaurus by Alberto Cairo, 2016 ·
<a href="https://www.research.autodesk.com/publications/same-stats-different-graphs/" target="_blank">
Same Stats, Different Graphs ↗
</a>
·
<a href="https://www.openintro.org/data/index.php?data=datasaurus" target="_blank">
Download dataset ↗
</a>
</div>

</div>

---
title: 02 · Structurer les données
level: 1
---

<div class="eyebrow">02 · Structurer les données</div>

# La forme compte

<div class="slide-intro">
Certaines structures sont faciles à lire pour nous, mais difficiles à exploiter.
</div>

<div class="full-visual">
  <img src="/assets/images/01-Extrait-Excel.png">
</div>

[Ouvrir le fichier Excel ↗](https://epflch-my.sharepoint.com/:x:/g/personal/genevieve_guex_epfl_ch/IQAaVC0B_0ybQ71Ul3AHfD8vAYURhc2NRJlpyHmimnIRiTE?e=d5V1xL){target="_blank" .demo-link


---


