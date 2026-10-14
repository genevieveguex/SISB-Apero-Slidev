---
theme: default
title: SISB — Heure de l'apéro
transition: fade
mdc: true
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

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

<div class="apero-page-number">{{ $page }}</div>

<div class="eyebrow">Sommaire</div>

# Aujourd’hui

<Toc minDepth="1" maxDepth="1" />

---
title: 01 · Voir autrement
level: 1
---

<div class="apero-page-number">{{ $page }}</div>

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

<div class="apero-page-number">{{ $page }}</div>

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

<div class="apero-page-number">{{ $page }}</div>

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

<div class="apero-page-number">{{ $page }}</div>

<div class="two-columns">

<div class="left-column">

<div class="eyebrow">01 · Introduction</div>

# Ce que vous ne voyez pas

*Existe-t-il une relation entre le nombre d'entrées  
et le nombre de prêts ?*

Les chiffres n’ont pas changé.  
La question que nous leur posons a changé.

</div>

<div class="right-column">
  <img src="/assets/images/01-03-Datasaurus.gif" alt="Visualisation Datasaurus">
</div>

</div>

---
title: P07-Voir autrement
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

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

<div class="apero-page-number">{{ $page }}</div>

<div class="title-slide">

<div class="eyebrow">02 · Repenser la structure</div>

# La forme <span class="underline">compte</span>.

<div class="subtitle">
Un tableau bien présenté n'est pas nécessairement un tableau facile à analyser.<br> 
Nos fichiers Excel sont souvent conçus pour être lus, beaucoup moins pour être exploités.
</div>

</div>

---
title: P09-La forme compte
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

<div class="eyebrow">02 · Repenser la structure</div>

# Votre avis : quelles sont le questions que nous pourrions poser à ce jeux de données?

<div class="full-visual">
  <img src="/assets/images/02-01-Excel-depart.png" alt="USEP Récolte Démo">
</div>

[Ouvrir le fichier Excel ↗](https://epflch-my.sharepoint.com/:x:/g/personal/genevieve_guex_epfl_ch/IQBPuv06uchVQJ63sRWYxpwLAd5uHcGlJFFlfFjigReckkM?e=jl0xg0){target="_blank" .demo-link}



---
title: P10-La forme compte
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

<div class="eyebrow">02 · Repenser la structure</div>

# Quelles sont les questions auxquelles <br> nous ne pouvons pas répondre?

  
**Évolution**
- quelle est la moyenne par trimestre?
- quel est le total par année académique (septembre-août)?
- quelle est la différence par rapport au mois précédent (nombre ou pourcentage)?
- quelle est la différence entre le nombre le plus haut et le nombre le plus bas (pourcentage)?

[Ouvrir le fichier Excel ↗](https://epflch-my.sharepoint.com/:x:/g/personal/genevieve_guex_epfl_ch/IQBPuv06uchVQJ63sRWYxpwLAd5uHcGlJFFlfFjigReckkM?e=jl0xg0){target="_blank" .demo-link}
  

---  
title: P11-La forme compte
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

<div class="eyebrow">02 · Repenser la structure</div>

# … et si nous désirons comparer 2026 <br> avec les années précédentes?	
  
**Saisonnalité**
- est-ce que le mois de mai est toujours celui avec le plus d'entrées?
- est-ce que nous avons une période durant laquelle les sollicitations sont plus hautes?

**Évolution**
- différence d'année en année (nombre, pourcent)

[Ouvrir le fichier Excel ↗](https://epflch-my.sharepoint.com/:x:/g/personal/genevieve_guex_epfl_ch/IQBPuv06uchVQJ63sRWYxpwLAd5uHcGlJFFlfFjigReckkM?e=jl0xg0){target="_blank" .demo-link}


---  
title: P12-La forme compte
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

<div class="eyebrow">02 · Repenser la structure</div>

# Le format des données doit changer

<div class="full-visual">
  <img src="/assets/images/02-02-Excel-Arrivee.png" alt="USEP Récolte Démo">
</div>

[Ouvrir le fichier Excel ↗](https://epflch-my.sharepoint.com/:x:/g/personal/genevieve_guex_epfl_ch/IQBPuv06uchVQJ63sRWYxpwLAd5uHcGlJFFlfFjigReckkM?e=jl0xg0){target="_blank" .demo-link}


---
title: 03-Power Query
level: 1
---

<div class="apero-page-number">{{ $page }}</div>

<div class="title-slide">

<div class="eyebrow">03 · Préparer les données</div>

# Faire le travail <span class="underline">une seule</span> fois.

<div class="subtitle">
Les données arrivent rarement dans le format qui nous arrange. <br>
Les fichiers ne sont pas statiques, de nouveaux éléments sont ajoutés en permanence.
</div>

Les transformations peuvent êtres sauvegardées et appliquées aux nouvelles tables. <br>

Découvrons **Power Query**.

</div>

---  
title: P14-Préparer les données
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

<div class="two-columns">

<div class="left-column">

<div class="eyebrow">03 · Préparer les données</div>

# Partir d'un fichier excel
Nous allons faire une démonstration du principe.

Power Query vit à l'intérieur d'Excel, dans l'onglet `données`.  
Vous y trouverez les options courantes, selon le type de fichier que vous voulez retravailler.


</div>


<div class="right-column">
  <img src="/assets/images/03-01-PQ-ouvrir.png" alt="Power Query">
</div>

</div>


---
title: P16-Préparer les données
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

<div class="two-columns">

<div class="left-column">

<div class="eyebrow">03 · Préparer les données</div>

# Go!

Nous continuons avec USEP. Dans la fenêtre popup nous sélectionnons le fichier Excel.

<div v-click="1">

Power Query lit votre fichier et vous propose  
des éléments à travailler :

- les tables
- les feuilles | onglets

</div>

</div>

<div class="right-column visual-fade">

  <img
    v-click-hide="1"
    class="visual-fade-image"
    src="/assets/images/03-02-PQ-choisir.png"
    alt="Options de connexion Power Query"
  />

  <img
    v-click="1"
    class="visual-fade-image"
    src="/assets/images/03-03-Choix-Table.png"
    alt="Sélection d'une table"
  />

</div>

</div>

---
title: P16-Préparer les données
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

<div class="eyebrow">03 · Préparer les données</div>

# Ouch.

Bli bla blo

<div class="visual-fade visual-full-width">

  <img
    v-click-hide="1"
    class="visual-fade-image"
    src="/assets/images/03-04-PQ-Interface.png"
    alt="Interface Power Query"
  />

  <img
    v-click="1"
    class="visual-fade-image"
    src="/assets/images/03-05-PQ-Interface-Note.png"
    alt="Sélection d'une table"
  />

</div>

---
title: P17-Préparer les données
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

<div class="eyebrow">03 · Préparer les données</div>

# Rappel - nous voulons arriver à ceci

<div class="right-column">
  <img src="/assets/images/03-01-PQ-ouvrir.png" alt="Power Query">
</div>

---
title: P18-Préparer les données
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>



<div class="eyebrow">03 · Préparer les données</div>

# Les étapes

maintenant que nous avons vérifié que notre table est bien chargée,
revenons en arrière

<div class="full-visual">
  <img src="/assets/images/03-06-Step-Back.gif" alt="Power Query">

</div>


---
title: P19-Préparer les données
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

<div class="two-columns">

<div class="left-column">

<div class="eyebrow">03 · Préparer les données</div>

# Étape 01 - garder les tables

Nous avons trouvé le moyen de charger toutes les tables existantes dans notre fichier.

Nous ne gardons que celles dont le type (`Kind`) est `Table`.

Filtrer se passe comme dans excel, en cliquant sur la petite flèche ▼, à droite du nom de la colonne à filtrer.
</div>

<div class="right-column">

<div class="images-vertical">

  <img src="/assets/images/03-07-Tables.png" alt="Tables Power Query">

  <img src="/assets/images/03-08-Filtrer.gif" alt="Filtrage Power Query">

</div>

</div>

</div>

---
title: P20-Préparer les données
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>


<div class="eyebrow">03 · Préparer les données</div>

# Étape 02 - extraire les informations

<div class="full-visual">

  <img src="/assets/images/03-10-Extraire.gif" alt="Tables Power Query">

</div>
