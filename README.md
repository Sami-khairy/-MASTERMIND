# Master Mind Game

### **Description**
Master Mind est un jeu interactif développé en langage C. Deux joueurs s'affrontent pour deviner un code numérique dans un temps limité. Ce jeu propose deux niveaux de difficulté, un système de joker et une sauvegarde des scores. Le projet a été conçu pour offrir une expérience utilisateur engageante grâce à des couleurs, animations et instructions interactives.

---

### **Table des Matières**
1. [Introduction](#introduction)
2. [Installation](#installation)
3. [Utilisation](#utilisation)
4. [Fonctionnalités](#fonctionnalités)
5. [Exemples d'Utilisation](#exemples-dutilisation)
6. [Structure du Code](#structure-du-code)
7. [Dépendances](#dépendances)
8. [Configuration](#configuration)
9. [Troubleshooting](#troubleshooting)
10. [Contributeurs](#contributeurs)
11. [Licence](#licence)

---

### **Introduction**
**Master Mind** est un jeu de logique où un joueur définit un code secret, et l'autre joueur doit le deviner en un nombre limité de tentatives. À chaque essai, des indices sont donnés sur les chiffres bien placés et ceux mal placés. 

Ce projet est réalisé en C, avec une attention particulière portée à l'interactivité et à l'engagement utilisateur.

---

### **Installation**
1. **Prérequis :**
   - Un compilateur C (GCC, MinGW, etc.).
   - Un terminal compatible avec les commandes système de Windows.
2. **Étapes d'installation :**
   - Téléchargez ou clonez le projet.
   - Placez le fichier source (`mastermind.c`) dans un répertoire local.
   - Compilez le fichier source avec la commande :
     ```bash
     gcc mastermind.c -o mastermind
     ```
   - Lancez le jeu avec :
     ```bash
     ./mastermind
     ```

---

### **Utilisation**
1. Lancez le jeu via le terminal ou l'invite de commande.
2. Suivez le menu principal :
   - **[1] Jouer** : Commencez une partie.
   - **[2] Règles** : Consultez les règles du jeu.
   - **[3] Quitter** : Quittez le programme.
3. Sélectionnez un niveau de difficulté :
   - Niveau 1 : Les chiffres du code ne peuvent pas se répéter.
   - Niveau 2 : Les chiffres peuvent se répéter.
4. Essayez de deviner le code en utilisant les indices donnés !

---

### **Fonctionnalités**
- **Deux niveaux de difficulté :**
  - *Niveau 1 :* Chiffres distincts.
  - *Niveau 2 :* Chiffres pouvant se répéter.
- **Système de Joker :**
  - Débloqué après un certain nombre d’essais restants.
  - Révélation d’un chiffre en échange de 3 essais.
- **Enregistrement des scores :**
  - Sauvegarde des résultats dans un fichier texte dans un répertoire dédié.
- **Interface interactive :**
  - Utilisation de couleurs, animations et messages dynamiques pour améliorer l'expérience utilisateur.
- **Compatibilité Windows :**
  - Exploitation de commandes système et gestion des couleurs via la console.

---

### **Exemples d'Utilisation**
Voici des captures d'écran montrant l'interface du jeu et ses fonctionnalités.

#### **1. Menu Principal**
![Menu Principal](D:\github\mastermaind_images\1.png)

#### **2. Entrée des Joueurs**
![Entrée des Joueurs](D:\github\mastermaind_images\2.png)

#### **3. Résultats d'une Partie**
![Résultats d'une Partie](D:\github\mastermaind_images\3.png)

#### **4. Sauvegarde des Scores**
![Fichier de Scores](D:\github\mastermaind_images\4.png)


---

### **Structure du Code**
- `main()` : Point d'entrée du programme.
- **Fonctions principales :**
- `Welcome` : Affiche le message d'accueil.
- `diff_printf` : Gère les couleurs et les caractères spéciaux.
- `Niveaux` : Navigation entre Niveau 1 et Niveau 2.
- `Joueur1_n1`, `Joueur2_n1` : Logique du jeu pour le Niveau 1.
- `Joueur1_n2`, `Joueur2_n2` : Logique du jeu pour le Niveau 2.
- `File` : Sauvegarde des scores dans un fichier texte.
- `Joker` : Gère l'activation et l'utilisation du joker.
- `Loading` : Animation de chargement.
- `Perdu` : Affiche le message de défaite.

---

### **Dépendances**
Le projet repose sur les bibliothèques standards suivantes :
- `stdio.h` : Gestion des entrées et sorties.
- `stdlib.h` : Gestion de la mémoire et commandes système.
- `windows.h` : Gestion des couleurs et commandes spécifiques à Windows.
- `time.h` : Gestion de la date et de l'heure.
- `conio.h` : Utilisation de `getch()` pour les entrées clavier.

---

### **Configuration**
- **Plateforme cible :** Windows (utilisation de commandes comme `cls`, `Sleep`, etc.).
- **Compilation :** Compatible avec GCC/MinGW.
- **Dossier de sortie :** Un répertoire `MasterMind` est créé automatiquement pour stocker les scores.

---

### **Troubleshooting**
1. **Couleurs non affichées correctement :**
 - Vérifiez que vous utilisez une console Windows compatible.
2. **Erreur de fichier :**
 - Assurez-vous d’avoir les permissions d’écriture dans le répertoire où vous exécutez le programme.
3. **Entrées invalides :**
 - Respectez les consignes (uniquement des chiffres entre 0 et 9).

---

### **Contributeurs (2021-2022) **
- **Sami Khairy**  
Étudiant en informatique à l'ESTC.
- **Haitam Benzinane**  
Étudiant en informatique à l'ESTC.
- **Issam Elkaamouse**  
Étudiant en informatique à l'ESTC.

---

### **Licence**
Ce projet est distribué sous licence libre. Vous êtes libre de le modifier et de le redistribuer à des fins éducatives ou personnelles.

---

### **Conclusion**
Le jeu **Master Mind** est une application amusante et interactive démontrant les compétences en programmation C. Il est parfait pour une utilisation éducative ou pour les amateurs de jeux de logique.

---

