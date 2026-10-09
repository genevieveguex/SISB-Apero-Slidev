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
title: P02-TOC
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
Les données ne parlent pas d'elles-mêmes. Encore faut-il savoir comment les regarder.

</div>

</div>

---
title: P04-Voir autrement
hideInToc: true
---

<div class="eyebrow">01 · Introduction</div>

# Les chiffres ne disent pas tout


<div class="full-visual">
  <img src="/assets/images/01-01-Extrait-Excel.png">
</div>

[Ouvrir le fichier Excel ↗](https://epflch-my.sharepoint.com/:x:/g/personal/genevieve_guex_epfl_ch/IQAaVC0B_0ybQ71Ul3AHfD8vAYURhc2NRJlpyHmimnIRiTE?e=d5V1xL){target="_blank" .demo-link}

Deux indicateurs de la Bibliothèque : entrées et prêts physiques.
Que pouvons-nous en déduire?


---
title: P05-Voir autrement
hideInToc: true
---

<div class="two-columns">

<div class="left-column">

<div class="eyebrow">01 · Introduction</div>

# Ce que vous voyez

*Comment les entrées et les prêts évoluent-ils* <br>
*dans le temps ?*

La visualisation transforme des valeurs en formes, écarts et relations que nous pouvons comparer.

</div>

<div class="right-column">
  <img src="/assets/images/01-02-LineChart.gif">
</div>

</div>

---
title: P06-Voir autrement
hideInToc: true
---

<div class="two-columns">

<div class="left-column">

<div class="eyebrow">01 · Introduction</div>

# Ce que vous ne voyez pas

*Existe-t-il une relation entre le nombre d'entrées* <br>
*et le nombre de prêts ?*

Les chiffres n’ont pas changé.  
La question que nous leur posons a changé.

</div>

<div class="right-column">
  <img src="/assets/images/01-03-Datasaurus.gif">
</div>

</div>

---
title: P07-Voir autrement
hideInToc: true
---

<div class="two-columns">

<div class="left-column">

<div class="eyebrow">01 · Introduction</div>

# Changer de point de vue

La première visualisation n'est pas nécessairement la bonne. C'est souvent simplement la première.


<p v-click="1">
Explorer, comparer, changer d'échelle ou de perspective permet de découvrir ce que notre première lecture avait laissé de côté.
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
Les données arrivent rarement dans le format qui nous arrange.

Un tableau bien présenté n'est pas nécessairement un tableau facile à analyser.<br> 
Nos fichiers Excel sont souvent conçus pour être lus, beaucoup moins pour être exploités.
</div>

</div>

---
title: P09-La forme compte
hideInToc: true
---

