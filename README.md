```markdown
# miniRT - 42 School Project

## 📋 Description
miniRT est un projet graphique avancé de 42 qui consiste à créer un moteur de rendu 3D capable de générer des images réalistes en utilisant la technique du ray tracing. Ce projet explore les concepts fondamentaux de l'infographie et du rendu photoréaliste.

## 🎯 Objectifs
- Implémenter un moteur de ray tracing basique
- Comprendre les mathématiques de la 3D et de l'éclairage
- Maîtriser les transformations géométriques
- Développer un parser pour fichiers de scène

## 🛠️ Technologies Utilisées

### 🎨 Graphisme
- **MiniLibX** - Bibliothèque graphique de 42
- **Ray Tracing** - Algorithme de rendu photoréaliste
- **Calcul vectoriel** - Opérations sur vecteurs et matrices

### 📐 Mathématiques
- **Géométrie 3D** - Intersections rayon/objets
- **Algèbre linéaire** - Transformations et projections
- **Théorie des couleurs** - Modèles RGB et éclairage

## 🚀 Installation et Utilisation

### 📋 Compilation
```bash
git clone [URL-du-repository]
cd miniRT
make
```

### ⚙️ Utilisation
```bash
# Rendu d'une scène
./miniRT scenes/scene.rt

# Sauvegarde en format BMP
./miniRT scenes/scene.rt --save
```

## 📊 Fonctionnalités Implémentées

### 🎭 Objets 3D Supportés
- **Sphères** - Objet géométrique basique
- **Plans** - Surfaces infinies
- **Cylindres** - Avec capsules optionnelles
- **Carrés** et **Rectangles** - Surfaces planes limitées
- **Triangles** - Géométrie polygonale

### 💡 Système d'Éclairage
- **Lumière ambiante** - Éclairage de base de la scène
- **Lumières directionnelles** - Sources de lumière ponctuelles
- **Lumières parallèles** - Éclairage directionnel
- **Modèle de Phong** - Diffusion, spécularité, ombres

### 🎨 Caractéristiques des Matériaux
- **Couleurs RGB** - Définition des matériaux
- **Reflets** - Composante spéculaire
- **Textures** - Couleurs unies (extension basique)

## 💡 Compétences Développées
- Programmation graphique 3D avancée
- Mathématiques pour l'infographie
- Algorithmes de ray tracing
- Parsing de fichiers de configuration
- Optimisation des performances
- Gestion de la mémoire pour scènes complexes

## 📁 Format des Fichiers .rt

### 🏗️ Éléments de Scène
```bash
# Résolution
R 1920 1080

# Lumière ambiante
A 0.2 255,255,255

# Caméra
C 0,0,0 0,0,1 70

# Lumière
L -40,0,30 0.6 255,255,255

# Sphère
sp 0,0,20 10 255,0,0

# Plan
pl 0,0,0 0,1,0 0,128,255

# Cylindre
cy 20,0,10 0,1,0 5 20 255,255,0
```

## 🎯 Fonctionnalités Avancées

### 🔧 Transformations
- **Multi-caméras** - Changement de viewpoint
- **Résolution configurable** - Adaptation à l'écran
- **Export BMP** - Sauvegarde des rendus

### 🛡️ Validation
- **Parser robuste** - Détection des erreurs de syntaxe
- **Validation des scènes** - Cohérence des paramètres
- **Gestion des erreurs** - Messages informatifs

## 📁 Structure du Projet
```
miniRT/
├── sources/
│   ├── exec/        # Moteur de ray tracing
│   ├── parsing/     # Parser de fichiers .rt
│   └── init/     
├── include/         # Fichiers d'en-tête
├── scenes/          # Fichiers de scène d'exemple
├── Makefile         # Système de compilation
```

Ce projet représente le sommet des compétences graphiques dans le cursus 42 et démontre une compréhension approfondie des techniques de rendu 3D moderne.
```
