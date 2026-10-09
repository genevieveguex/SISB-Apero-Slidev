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
title: 01 · Voir autrement
level: 1
---

<div class="title-slide">

<div class="eyebrow">01 · INTRODUCTION</div>

# Voir `[autrement]`

<div class="subtitle">
De la question à la visualisation : démonstration d’un workflow<br>
<strong>Excel → Power Query → Power Pivot | Power BI</strong><br>
en explorant quelques fonctionnalités méconnues des outils Microsoft.
</div>

</div>

---
title: P04-Voir Voir autrement
hideInToc: true
---

<div class="eyebrow">01 · Introduction</div>

# Voir `[autrement]`

Les données brutes décrivent une réalité, mais elles ne la rendent pas immédiatement visible.

<div class="full-visual">
  <img src="/assets/images/01-01-Extrait-Excel.png">
</div>

[Ouvrir le fichier Excel ↗](https://epflch-my.sharepoint.com/:x:/g/personal/genevieve_guex_epfl_ch/IQAaVC0B_0ybQ71Ul3AHfD8vAYURhc2NRJlpyHmimnIRiTE?e=d5V1xL){target="_blank" .demo-link}

Face au tableau, notre cerveau doit lire, mémoriser et comparer une succession de nombres.

---
title: P05-Voir Voir autrement
hideInToc: true
---

<div class="two-columns">

<div class="left-column">

<div class="eyebrow">01 · Introduction</div>

# Ce que vous voyez

La visualisation transforme des valeurs en formes, écarts et relations que nous pouvons comparer.

Le graphique donne une forme aux données.  
Tendances, écarts et relations deviennent visibles.

</div>

<div class="right-column">
  <img src="/assets/images/01-02-LineChart.gif">
</div>

</div>

---
title: P06-Voir Voir autrement
hideInToc: true
---

<div class="two-columns">

<div class="left-column">

<div class="eyebrow">01 · Introduction</div>

# Ce que vous ne voyez pas

Les chiffres n’ont pas changé.  
La question que nous leur posons a changé.

Une autre question fait apparaître une autre structure dans les mêmes données.

</div>

<div class="right-column">
  <img src="/assets/images/01-03-Datasaurus.gif">
</div>

</div>

---
title: P07-Voir Voir autrement
hideInToc: true
---

<div class="two-columns">

<div class="left-column">

<div class="eyebrow">01 · Introduction</div>

# Changer de point de vue

Une seule vue suffit rarement.

Comparer, vérifier et changer de perspective permet de mieux comprendre les données.

<p v-click="1">
Avant de conclure, il faut vérifier ce que l’on voit — et ce que l’on ne voit pas.
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
    src="/assets/images/01-05-Datasaurus.png"
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
title: 02 · La forme compte
level: 1
---

<div class="title-slide">

<div class="eyebrow">02 · Structurer les données</div>

# La forme <span class="underline">compte</span>

<div class="subtitle">
De la question à la visualisation : démonstration d’un workflow<br>
<strong>Excel → Power Query → Power Pivot | Power BI</strong><br>
en explorant quelques fonctionnalités méconnues des outils Microsoft.
</div>

</div>
