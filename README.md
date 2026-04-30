# 🛡️ RGPD Training Lab

Plateforme de formation interactive à la cybersécurité et à la conformité RGPD.  
**Un seul conteneur Docker, un seul port, navigation 100% locale.**

---

## 🚀 Démarrage rapide

```bash
# Cloner le repo
git clone https://github.com/asepol/CyberPrivacy-Training-Lab
cd CyberPrivacy-Training-Lab

# Lancer
docker compose up -d --build

# Accéder à la plateforme
http://localhost:8080
```

---

## 📦 Architecture

```
rgpd-training/
├── docker-compose.yml        → Un seul service, un seul port (8080)
├── Dockerfile                → Image nginx:alpine
├── nginx.conf                → Config Nginx (gzip, cache, headers sécurité)
└── site/
    ├── index.html            → Portail principal (progression guidée, badges, XP)
    ├── tp1-identite.html     → TP interactif — Identité numérique & DCP
    ├── tp2-bonnes-pratiques.html → TP interactif — Bonnes pratiques & sécurité
    ├── tp3-fuite.html        → TP interactif — Fuite de données
    └── tp4-cybercrise.html   → TP interactif — Cyber-crise & gouvernance
```

---

## 🎯 Modules de formation

| # | Module | Thèmes | Niveau |
|---|--------|--------|--------|
| 1 | 🧠 Identité numérique & DCP | Données personnelles, données sensibles, minimisation | 🌱 |
| 2 | 🛡️ Bonnes pratiques & sécurité | Art. 32, mots de passe, sauvegardes, règle 3-2-1 | 🧩 |
| 3 | 💥 Fuite de données | Notification CNIL 72h, art. 33/34, phishing | ⚠️ |
| 4 | 🚨 Cyber-crise & gouvernance | Cellule de crise, ransomware, accountability | 🔥 |
| 5 | 📑 Contrat de sous-traitance (DPA) | Art. 28, clauses obligatoires, sous-traitants ultérieurs | 📑 |
| 6 | 🧩 Privacy by Design | Art. 25, minimisation, opt-in, paramètres protecteurs | 🧩 |
| 7 | 🕵️ Dark Patterns & consentement | Art. 7, bannières cookies, CNIL 2022 | 🕵️ |
| 8 | 📘 Registre des traitements | Art. 30, accountability, contenu obligatoire | 📘 |
| 9 | 📊 DPIA (Analyse d'impact) | Art. 35, critères déclencheurs, liste CNIL | 📊 |
| 10 | 🧑‍⚖️ Droits des personnes | Art. 12-22, accès, effacement, opposition, portabilité | 🧑‍⚖️ |

---

## 🎮 Fonctionnalités pédagogiques

- **Progression séquentielle** — chaque module se débloque après validation du précédent
- **TPs interactifs** — formulaires fictifs, code d'audit, scénarios de crise, timelines
- **4 questions par mission** dont une mise en situation concrète
- **Feedback explicatif** — explication pédagogique après chaque réponse (bonne ou mauvaise)
- **Système XP + Badges** — 10 badges thématiques, niveaux Débutant → RGPD Ready
- **Récapitulatif de fin** — synthèse des compétences acquises à la complétion du parcours
- **Réinitialisation** — bouton pour recommencer depuis zéro (utile en mode formateur)
- **Durée estimée** — ~3h de formation complète

---

## ⚙️ Commandes utiles

```bash
# Lancer la plateforme
docker compose up -d --build

# Arrêter
docker compose down

# Voir les logs
docker compose logs -f

# Vérifier le statut
docker compose ps

# Rebuild après modification des fichiers
docker compose up -d --build
```

---

## 🔒 Principes techniques

- **Un seul conteneur** — Nginx sert tous les fichiers HTML statiques
- **Navigation locale** — tous les liens sont des `href` relatifs, aucun port externe
- **TPs inline** — les travaux pratiques s'affichent dans la même page via JavaScript
- **Progression** — sauvegardée en `localStorage` du navigateur
- **Aucune dépendance externe** — fonctionne sans internet après le `docker build`
- **Sécurité Nginx** — headers `X-Frame-Options`, `X-Content-Type-Options`, gzip activé

---

## 📚 Références réglementaires

- [Règlement RGPD (UE) 2016/679](https://eur-lex.europa.eu/legal-content/FR/TXT/?uri=CELEX%3A32016R0679)
- [CNIL — Guide pratique RGPD](https://www.cnil.fr/fr/rgpd-de-quoi-parle-t-on)
- [ANSSI — Guide de gestion de crise cyber](https://www.ssi.gouv.fr/guide/organiser-un-exercice-de-gestion-de-crise-cyber/)

---

## ⚠️ Avertissement

> Environnement de formation fictif. Aucune donnée saisie n'est réellement collectée ou stockée.  
> Les scénarios, entreprises et personnages mentionnés sont entièrement fictifs.

---

*Projet réalisé à des fins éducatives — Cybersécurité & conformité RGPD*
