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

[Ouvrir le fichier Excel Demo-01 ↗](https://epflch-my.sharepoint.com/:x:/g/personal/genevieve_guex_epfl_ch/IQB5HvAo5dGrQ62nm2qBVIHcAVtSpBlB-xpWGvWoCqfJZiI?e=vk0662){target="_blank" .demo-link}

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
title: P09-Repenser la structure
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

<div class="eyebrow">02 · Repenser la structure</div>

# Votre avis : quelles sont le questions que nous pourrions poser à ce jeux de données?

<div class="full-visual">
  <img src="/assets/images/02-01-Excel-depart.png" alt="USEP Récolte Démo">
</div>

[Ouvrir le fichier Excel Demo-02 ↗](https://epflch-my.sharepoint.com/:x:/g/personal/genevieve_guex_epfl_ch/IQD4DGUEi9wMT7F7UE6337lfAYyKty0dOSYo1gKj1xE1nYc?e=blsZ7N){target="_blank" .demo-link}



---
title: P10-Repenser la structure
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

<div class="eyebrow">02 · Repenser la structure</div>

# Pourquoi ne pouvons-nous pas aller plus loin? <br>

**Nous devons séparer le format visuel du format d'analyse et construire notre fichier différemment**
- nos valeurs doivent toutes se trouver dans une seule table
- la table doit se mettre à jour toute seule lorsque les valeurs sont modifiées




[Ouvrir le fichier Excel Demo-03 ↗](https://epflch-my.sharepoint.com/:x:/g/personal/genevieve_guex_epfl_ch/IQDTNlCQQseQTbtmRilDdHvXATcgg0JkWO0n7B7ukFSfTFw?e=asMefe){target="_blank" .demo-link}


---  
title: P11-La forme compte
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

<div class="eyebrow">02 · Repenser la structure</div>

# Le format des données doit changer

<div class="full-visual">
  <img src="/assets/images/02-02-Excel-Arrivee.png" alt="USEP Récolte Démo">
</div>

[Ouvrir le fichier Excel de départ ↗](https://epflch-my.sharepoint.com/:x:/g/personal/genevieve_guex_epfl_ch/IQB5GIJZ5GZyQYockbR11VZRAaaE5qfutF-6lp2tD4kpcI4?e=D44Dbz){target="_blank" .demo-link}

---
title: 03 · Extraire - Transformer - Charger
level: 1
---

<div class="apero-page-number">{{ $page }}</div>

<div class="title-slide">

<div class="eyebrow">03 · Extraire - transformer - charger</div>

# Faire le travail <span class="underline">une seule</span> fois.

<div class="subtitle">
Les données arrivent rarement dans le format qui nous arrange. <br>
Les sources ne sont pas statiques, de nouveaux éléments sont ajoutés en permanence.

Changer les formats des tables à chaque mise-à-jour n'est pas imaginable.
</div>

</div>

---
title: P13-ETL
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

<div class="eyebrow">03 · Extraire - transformer - charger</div>

<div class="full-visual">
  <img src="/assets/images/03-Slide-flux.png" alt="USEP Récolte Démo">
</div>




---
title: P14-ETL
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

<div class="eyebrow">03 · Extraire - transformer - charger</div>

# Power Query
Power Query permet d'importer, de combiner et de transformer des données provenant de différentes sources.


<div class="visual-full-width">
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
    alt="Interface Power Query annotée"
  />
</div>

Sans modifier les fichiers d'origine. Et sans devoir écrire une ligne de code.

[la liste complète ↗](https://learn.microsoft.com/en-us/power-query/connectors/){target="_blank" .demo-link}



---
title: P15-ETL
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

<div class="eyebrow">03 · Extraire - transformer - charger</div>

# Opérations de transformation courantes
Après avoir chargé vos différentes sources vous pouvez:

- réparer des structures (opérations sur lignes et colonnes)
- utiliser des délimiteurs pour extraire du texte
- créer des colonnes conditionnelles
- retravailler des formats de date
- calculer de nouvelles valeurs avec des opérations mathématiques

---
title: P16-ETL
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>
<div class="two-columns">

<div class="left-column">

<div class="eyebrow">03 · Extraire - transformer - charger</div>

# Démarrer la transformation

Power Query se lance depuis l'onglet `Données` d'excel. Vous pouvez l'utiliser :

- dans le même fichier que vos tables existantes,  
  dans ce cas vous choisirez  
`A partir d'un tableau ou d'une plage`

- dans un fichier vide que vous liez à vos sources:  
`A partir d'un fichier`  ou  
`A partir d'un dossier`  
pour récupérer plusieurs fichiers en vue d'un assemblage

</div>


<div class="right-column">
  <img src="/assets/images/03-02-LancerPQ.png" alt="USEP Récolte Démo">
</div>

</div>

[Ouvrir le fichier Excel avec les étapes ↗](https://epflch-my.sharepoint.com/:x:/g/personal/genevieve_guex_epfl_ch/IQCrj9uwrUZPRZcM-5qcYV2LAbTJD2QyJxhq8u3n5x8PJSM?e=mFM3nP){target="_blank" .demo-link}


---
title: P17-ETL
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

<div class="eyebrow">03 · Extraire - transformer - charger</div>

# Le résultat
Un fichier pratique pour la saisie et utilisable pour l'analyse
<div class="visual-full-width">
  <img
    v-click-hide="1"
    class="visual-fade-image"
    src="/assets/images/03-06-Resultat.png"
    alt="Résultat Power Query — étape 1"
  />

  <img
    v-click="[1, 2]"
    class="visual-fade-image"
    src="/assets/images/03-06-Resultat-B.png"
    alt="Résultat Power Query — étape 2"
  />

  <img
    v-click="2"
    class="visual-fade-image"
    src="/assets/images/03-06-Resultat-C.png"
    alt="Résultat Power Query — étape 3"
  />

</div>

<div class="visual-captions">
  <div v-click-hide="1">La présentation des données est séparée des données sources</div>
  <div v-click="[1, 2]">Les tables de récolte servent deux objectifs: saisir les valeurs et alimenter Power Query</div>
  <div v-click="2">La table de travail Power Query qui alimente les rapports vit dans son propre onglet</div>
</div>

[Ouvrir le fichier Excel terminé ↗](https://epflch-my.sharepoint.com/:x:/g/personal/genevieve_guex_epfl_ch/IQBK-dh-sWqvSZZ-dL0gr7bAAW_d72uWJrKV6gRC8Cg0SmM?e=px7R6z){target="_blank" .demo-link}


---
title: P18-ETL
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

<div class="eyebrow">03 · Extraire - transformer - charger</div>

# Et maintenant?
Nos données sont désormais structurées, exploitables et actualisables.

Mais elles ne racontent chacune qu'une partie de l'histoire.

Et si nous les faisions dialoguer ?


---
title: 04 · Organiser et enrichir
level: 1
---

<div class="apero-page-number">{{ $page }}</div>

<div class="title-slide">

<div class="eyebrow">04 · Organiser et enrichir</div>

# Tout est dans la <span class="underline">relation</span>.

<div class="subtitle">

Mettre des tables en mémoire.<br>
Les relier entre elles.  

C'est le modèle de données - aka modèle sémantique.

</div>
</div>

---
title: P20-ORGANISER ET ENRICHIR
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

<div class="two-columns">

<div class="left-column">

<div class="eyebrow">04 · Organiser et enrichir</div>

# Allons faire un tour
Les statistiques EPFL 2026 viennent d'être publiées.

Allons voir qui est notre public.

</div>

<div class="right-column">
  <img src="/assets/images/04-01-Stats_EPFL.png" alt="USEP Récolte Démo">
</div>

</div>

[Statistiques insitutionnelles de l'EPFL ↗](https://www.epfl.ch/about/data/fr/donnees-institutionnelles/statistiques-institutionnelles/){target="_blank" .demo-link}

---
title: P21-ORGANISER ET ENRICHIR
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

<div class="two-columns">

<div class="left-column">

<div class="eyebrow">04 · Organiser et enrichir</div>

# Allons faire un tour
Les statistiques EPFL 2026 viennent d'être publiées.
Voyons qui est notre public.
</div>

<div class="right-column">
  <img src="/assets/images/04-01-Stats_EPFL.png" alt="USEP Récolte Démo">
</div>

</div>

---
title: P21-ORGANISER ET ENRICHIR
hideInToc: true
---

<div class="apero-page-number">{{ $page }}</div>

# Comment savoir ce que j'ai téléchargé?
Un petit programme très pratique nous permet de voir et modifier des fichiers `*.csv`.

<div class="visual-full-width">
  <img
    v-click-hide="1"
    class="visual-fade-image"
    src="/assets/images/04-02-Stats_EPFL-Total.png"
    alt="Résultat Power Query — étape 1"
  />

  <img
    v-click="[1, 2]"
    class="visual-fade-image"
    src="/assets/images/04-02-Stats_EPFL-New.png"
    alt="Résultat Power Query — étape 2"
  />

  <img
    v-click="2"
    class="visual-fade-image"
    src="/assets/images/04-02-Stats_EPFL-Effectif.png"
    alt="Résultat Power Query — étape 3"
  />

</div>

<div class="visual-captions">

  <div v-click-hide="1">
    La table <code>Effectif total.csv</code> n'est pas très utile.
  </div>

  <div v-click="[1, 2]">
    La table <code>Effectif new.csv</code> peut éventuellement être utile.
  </div>

  <div v-click="2">
    La table <code>Table effectif.vsv</code> est bien et nous allons l'utiliser.
  </div>

</div>

[Smooth CSV ↗](https://smoothcsv.com/fr){target="_blank" .demo-link}