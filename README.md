# 🐍 Snake Game — Assembleur MIPS32

<br>

## 🧩 À propos du projet

Ce projet a été réalisé dans le cadre de ma **première année de BUT Informatique** à l’**IUT Robert Schuman**, sous la supervision d’enseignants.  
L’objectif est de **développer une version du jeu Snake** en **assembleur MIPS32**, en s’appuyant sur les principes fondamentaux de l’architecture des processeurs, de la mémoire et des appels système.

<br>

## 🎮 Description du jeu

Le jeu reprend le concept classique du **Snake** :
- Le joueur dirige un serpent sur une grille à l’aide des touches du clavier.  
- Le serpent **grandit à chaque bonbon mangé**.  
- Des **obstacles** apparaissent au fil de la partie.  
- Le jeu se termine lorsque le serpent **entre en collision** avec un mur, un obstacle ou lui-même.  
- Un **score** s’affiche à la fin de la partie.

<br>

## 👾 Commandes du jeu

| Touche | Action |
|:-------|:--------|
| **Z** | Monter |
| **S** | Descendre |
| **Q** | Aller à gauche |
| **D** | Aller à droite |

<br>

## ⚙️ Fonctionnalités principales

- 🐍 **Déplacement fluide** du serpent dans la grille  
- 🍬 **Gestion du bonbon** (apparition aléatoire et détection de collision)  
- 🧱 **Génération d’obstacles** après chaque bonbon mangé  
- 🧭 **Gestion des directions** (impossible de faire demi-tour)  
- 💥 **Détection de fin de jeu** :
  - Collision avec un mur  
  - Collision avec un obstacle  
  - Collision avec soi-même  
- 🧮 **Affichage du score final** avec un message personnalisé  

<br>

## 🧠 Concepts d’architecture utilisés

- Manipulation de **registres MIPS ($t, $s, $a, $v)**  
- Gestion de la **pile (stack)** pour les appels de fonctions (`$sp`, `sw`, `lw`)  
- Utilisation des **syscalls** pour les entrées/sorties  
- Emploi de **boucles et conditions** (`beq`, `bne`, `j`, `jr`, etc.)  
- Organisation en **sections `.data` et `.text`**  
- Représentation du plateau de jeu dans un **frame buffer mémoire**

<br>

## 🛠️ Technologies et environnement

- **Langage :** Assembleur MIPS32  
- **Émulateur recommandé :** [MARS MIPS Simulator](https://courses.missouristate.edu/kenvollmar/mars/)
- **Système :** Compatible avec tout environnement supportant MIPS32 (Windows, Linux, macOS)

<br>

## 🚀 Lancer le jeu

### 1️⃣ Ouvrir le projet dans MARS

1. Télécharger le fichier source (ex. `snake.asm`)  
2. Ouvrir le fichier dans **MARS** 
3. Assembler le programme (`Assemble`)  
4. Lancer l’exécution (`Run`)

> 💡 Conseil : Activez l’affichage graphique dans MARS pour voir la grille se mettre à jour (framebuffer intégré au code).
