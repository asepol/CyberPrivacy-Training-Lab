# 🛡️ CyberPrivacy Training Lab

Un laboratoire interactif conçu pour sensibiliser le public aux enjeux de la cybersécurité, de la protection des données personnelles et du RGPD.  
Ce projet propose un parcours ludique, pédagogique et accessible à tous.

---

## 🎯 Objectifs du projet

- Comprendre les risques liés à la vie privée en ligne  
- Apprendre les bons réflexes de cybersécurité  
- Identifier les données personnelles sensibles  
- Découvrir les principes essentiels du RGPD  
- S’entraîner via des scénarios interactifs et des mini‑jeux  

---

## 🧩 Contenu du Lab

- **Modules pédagogiques** : vidéos, quiz, fiches pratiques  
- **Scénarios interactifs** : phishing, mots de passe, réseaux sociaux  
- **Ateliers pratiques** : analyse de données, bonnes pratiques  
- **Tableau de progression** : score, badges, niveaux  

---

## 🚀 Installation

### 🔧 Installation locale

```bash
git clone https://github.com/asepol/CyberPrivacy-Training-Lab.git
cd CyberPrivacy-Training-Lab
```
### 🐳 Installation via Docker
```
apt install docker.io
apt install docker-compose

Dans le dossier --> CyberPrivacy-Training-Lab
docker compose -d --build
```
Le lab sera accessible sur :
👉 http://localhost:9000

### 🛠️ Technologies utilisées
- HTML / CSS / JavaScript
- Docker
- Nginx

### 📂 Structure du projet
```bash
CyberPrivacy-Training-Lab/
│
├── assets/           # Images, icônes, ressources
├── modules/          # Modules pédagogiques
├── scenarios/        # Exercices et mini-jeux
├── index.html        # Page principale
├── Dockerfile        # Build Docker
└── README.md
```
### 🕵️‍♂️ Missions du Lab

Le Lab propose plusieurs missions interactives permettant d’apprendre en s’amusant :

- **Mission 1 — Identité numérique & DCP**  
  Explorez un faux site de collecte de données et identifiez les données à caractère personnel, les excès de collecte et les risques associés.

- **Mission 2 — Bonnes pratiques & sécurité**  
  Analysez un intranet fictif rempli de mauvaises pratiques : mots de passe, accès, sauvegardes, et proposez des mesures correctives.

- **Mission 3 — Fuite de données**  
  Faites face à une fuite de données simulée : fichiers exposés, e-mails suspects, données sensibles. Analysez, qualifiez et proposez les actions RGPD.

- **Mission 4 — Cyber-crise & gouvernance**  
  Vivez une mini cyber-crise : prenez des décisions, priorisez les actions, et voyez l’impact sur la conformité et la réputation.

- **Mission 5 — Contrat de sous-traitance (DPA)**  
  Analysez un contrat de sous-traitance fictif et identifiez les clauses manquantes ou insuffisantes au regard du RGPD.

- **Mission 6 — Privacy by Design**  
  Analysez une interface volontairement mal conçue et identifiez les violations des principes de Privacy by Design et by Default.

- **Mission 7 —  Dark Patterns & consentement**  
  Identifiez les manipulations UX (dark patterns) qui biaisent le consentement ou la gestion des cookies sur un site fictif.
  
- **Mission 8 — Registre des traitements **  
  Analysez un registre de traitements fictif, repérez les incohérences et proposez des corrections pour le rendre conforme.
  
- **Mission 9  — DPIA (Analyse d’impact)**  
  Évaluez un projet à risque (vidéosurveillance, scoring, géolocalisation) et déterminez si une DPIA est nécessaire, ainsi que les mesures à prévoir.
  
- **Mission 10  — Droits des personnes**  
  Simulez la gestion d’une demande d’accès, de rectification ou d’effacement, et identifiez les bonnes pratiques de réponse.
---
