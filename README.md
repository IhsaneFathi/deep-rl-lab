# 🧠 Deep RL Lab — Laboratoire Interactif de Deep Reinforcement Learning

> *Un parcours d'apprentissage complet sur le Deep Reinforcement Learning — interactif, visuel, et progressif.*

**By [IHSANE FATHI](https://github.com/ihsanefathi)** 🦋🌹

---

## ✨ Aperçu

**Deep RL Lab** est une plateforme pédagogique entièrement autonome (un seul fichier `.html`) conçue pour apprendre le Deep Reinforcement Learning de façon active : vous ne lisez pas — vous simulez, vous expérimentez, vous répondez.

Pas de serveur. Pas d'installation. Ouvrez le fichier, apprenez.

---

## 🗺️ Structure du parcours

Le lab est organisé en **9 modules progressifs** + un tableau de bord et une arène finale, tous déverrouillables par l'apprenant :

| Module | Titre | Contenu clé |
|--------|-------|-------------|
| 0 | Tableau de Bord | Vue d'ensemble, XP, roadmap |
| 1 | Fondations du Deep RL | Agent, état, action, récompense, politique |
| 2 | Réseaux de Neurones | Approximation des Q-valeurs, forward pass |
| 3 | Deep Q-Networks (DQN) | Architecture, ε-greedy, exploration |
| 4 | Techniques d'Optimisation | Replay Buffer, Target Network |
| 5 | Algorithmes DQN Avancés | Double DQN, Dueling DQN, PER |
| 6 | Policy Gradient | REINFORCE, Actor-Critic, variance |
| 7 | PPO & TRPO | Clipping, région de confiance |
| 8 | Outils & Bibliothèques | Gym, PyTorch, Stable Baselines 3, RLlib |
| 9 | Arène Finale | Comparaison des algorithmes, cas pratiques |

---

## 🎮 Fonctionnalités interactives

### Simulations intégrées
- **Environnement Warehouse** (Module 1–3) — Agent naviguant en grille avec récompenses en temps réel
- **Visualisation Réseau de Neurones** (Module 2) — Forward pass animé, activation des couches
- **Contrôle ε-greedy** (Module 3) — Ajustez ε et observez l'équilibre exploration/exploitation
- **Réglage du Target Network C** (Module 4) — Stabilité vs vitesse selon la fréquence de mise à jour
- **REINFORCE vs Actor-Critic** (Module 6) — Visualisation live de la réduction de variance
- **Politique stochastique** (Module 6) — Observez π(a|s) évoluer après chaque récompense
- **PPO Clip Ratio** (Module 7) — Sliders interactifs pour voir le clipping en action

### Système de progression
- 🏅 **Points XP** accumulés à chaque module complété
- 🔒 **Modules verrouillés** — chaque module se débloque après le précédent
- ✅ **Quiz de raisonnement** — 3 questions par module avec feedback explicatif
- 📊 **Barre de progression** globale en temps réel

---

## 🚀 Utilisation

```bash
# Cloner le dépôt
git clone https://github.com/ihsanefathi/deep-rl-lab.git
cd deep-rl-lab

# Ouvrir dans le navigateur (aucune installation requise)
open index.html
```

Ou simplement **télécharger le fichier `.html`** et l'ouvrir dans n'importe quel navigateur moderne.

> ✅ Compatible Chrome, Firefox, Safari, Edge — aucune dépendance externe (sauf Google Fonts)

---

## 🛠️ Stack technique

Le lab est entièrement contenu dans **un seul fichier HTML** sans framework ni bundler :

- **HTML5 / CSS3** — mise en page responsive, variables CSS, animations
- **JavaScript vanilla** — toutes les simulations, le moteur de quiz, le système XP
- **Canvas API** — animation de la signature 
- **Google Fonts** — Cormorant Garamond, DM Sans, DM Mono
- **Zéro dépendance** — aucun npm, aucun build step

---

## 📐 Architecture du code

```
index.html
├── <style>              # ~900 lignes — design system complet (variables, composants)
├── <body>
│   ├── .sidebar         # Navigation + barre XP
│   └── .main
│       ├── #page-0      # Dashboard
│       ├── #page-1..9   # Modules 1 à 9
│       └── #page-10     # Résultats finaux
└── <script>             # ~1200 lignes
    ├── STATE            # Gestion de la progression (localStorage-free)
    ├── QUIZZES          # Données des quiz (m1–m9)
    ├── NAVIGATION       # Déverrouillage progressif
    ├── RENDER           # Rendu dynamique (nav, quiz, pages)
    ├── initLab1()       # Simulation Warehouse
    ├── initNNViz()      # Visualisation réseau neuronal
    ├── initDQN()        # Simulation ε-greedy + Replay Buffer
    ├── initActorCriticSim()  # REINFORCE vs AC variance
    ├── initPolicySim()       # Politique stochastique
    ├── initPPOSim()          # PPO clip ratio
    └── initSignatureCanvas() # Animation papillons & roses
```

---

## 📸 Captures d'écran

| Dashboard | Simulation DQN | Quiz |
|-----------|---------------|------|
|<img width="944" height="435" alt="dashboard" src="https://github.com/user-attachments/assets/6fd7786b-966d-46ec-9e6e-e4b28afaf2ae" /> | <img width="869" height="437" alt="quiz" src="https://github.com/user-attachments/assets/330a141e-0a7e-4543-9cc0-42ecd36ca4f3" /> | <img width="797" height="314" alt="simulation" src="https://github.com/user-attachments/assets/15dd0876-15eb-442a-b2eb-c82df58a0676" /> |

---

## 🎯 Public cible

- Étudiants 
- Ingénieurs souhaitant consolider leurs bases en RL
- Toute personne curieuse du Deep RL, même sans background mathématique profond

---

## 📄 Licence

Ce projet est distribué sous licence **MIT**.
Libre d'utilisation, de modification et de redistribution avec attribution.

```
MIT License — Copyright (c) 2025 Ihsane Fathi
```

---

## 🌹 À propos de l'auteure

Créé avec soin par **Ihsane Fathi** — Étudiante ingénieure passionnée par la pédagogie active et la transmission des savoirs

> *"On n'apprend pas en regardant. On apprend en faisant."*

---

<div align="center">
  🦋 &nbsp;&nbsp; 🌹 &nbsp;&nbsp; 🦋
  <br><br>
  <sub>Made with passion · Deep RL Lab</sub>
</div>
