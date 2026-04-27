Qu'est-ce qu'Arena Hub ?

**La plateforme tout-en-un pour organiser et analyser tes événements gaming.**

Arena Hub permet aux joueurs, équipes et créateurs gaming d’organiser facilement leurs tournois, scrims, leagues et collabs tout en suivant leurs performances en jeu, le tout dans un seul espace centralisé.

📖 À propos du projet

Arena Hub vise à remplacer la stack chaotique actuelle :
Discord + Google Sheets + Notion + Start.gg/Challonge + trackers divers

Notre vision : Une seule plateforme pour gérer communauté, événements et performances.


## ✨ Fonctionnalités principales

### 🔐 Authentification & Utilisateurs
- Inscription / Connexion email + mot de passe
- Changement de mot de passe
- Profil (nom affiché, bio, mode Streamer)
- Contrôle d'accès par plan (`FREE` / `STARTER` / `PRO` / `ENTERPRISE`)
- Rôle **Super Admin** avec surcharges illimitées
- Gestion utilisateurs admin (ban, plan, recherche)

### 👥 Social & Amis
- Demandes d'amis (envoyer, accepter, refuser, bloquer)
- Liste d'amis avec états (en attente / envoyé / accepté)
- Suppression d'amis
- Notifications de demandes d'amis

### 👥 Groupes
- Création de groupes temporaires (24h) et permanents
- Système d'invitation par code
- Gestion des membres avec rôles (`OWNER`, `ADMIN`, `PLAYER`, `COACH`, `REFEREE`, `CASTER`, `STAFF`…)
- Rôles in-game personnalisés par membre
- Sessions de groupe (start / end)
- Archivage de groupe
- Capacité max selon le plan : `FREE:20` · `STARTER:50` · `PRO:999`
- Expiration automatique des groupes temporaires

### 🎯 Événements
- Création d'événements public/privé avec statuts (`DRAFT`, `PUBLISHED`, `LIVE`, `ENDED`, `CANCELLED`)
- Types : `TOURNAMENT`, `SCRIMMAGE`, `LEAGUE`, `CHARITY`, `COLLAB`, `CUSTOM`
- Gestion des membres avec permissions par rôle
- Système de check-in
- Invitations utilisateurs avec notifications
- Intégration Discord Webhook
- Navigation des événements publics

### 🏆 Brackets & Tournois
- Formats : `SINGLE_ELIMINATION`, `DOUBLE_ELIMINATION`, `ROUND_ROBIN`, `SWISS`
- Génération automatique du bracket
- Gestion des rounds et matchs
- Résultats avec scores et vainqueurs
- Seeding des participants

### 📋 Tasks & Kanban
- Colonnes `TODO` / `IN_PROGRESS` / `DONE`
- Création avec titre, description, dates d'échéance
- Assignation aux membres
- Drag & drop
- Mises à jour temps réel via WebSocket

### 📊 Matchs & Statistiques
- Création de matchs avec stats détaillées (kills, deaths, assists, damage, healing, score, placement)
- Log des kill events (killer, victim, weapon, round, timestamp)
- Types : `RANKED`, `CASUAL`, `TOURNAMENT`
- Agrégation de stats joueur
- Stats duo et head-to-head
- Classements globaux (leaderboards)

### 🎮 Riot Games (Valorant · LoL · TFT)

> **⚠️ État RSO (Riot Sign-On) : En attente d'approbation par Riot Games**

- Liaison de compte Riot (gameName#tagLine)
- ~~OAuth2 PKCE complet (RSO)~~ → **En attente de validation par l'équipe Riot**
- Fallback manuel via Henrik API (sans OAuth)
- Sync automatique de l'historique de matchs
- Support multi-jeu : `VALORANT`, `LOL`, `TFT`
- Stats par jeu : agent/champion, map, mode, round, rang, HS%, placement TFT
- Affichage rang Valorant (Fer → Radiant)
- `RiotAccountCard` avec statut de liaison

📡 Live Dashboard & Temps Réel
- Scoreboard live des matchs en cours (équipes Bleue/Rouge, KDA)
- Données client local LoL/TFT via port 2999 (Live Client Data API)
- Corrélation PUUID → profil Arena Hub en direct
- Mises à jour temps réel via WebSocket (namespace `/dashboard`)
- Toasts de fin de match
- Affichage couleurs agents Valorant

🖥️ Arena Agent (Plugin)
- Création et gestion de tokens (`CLIENT` / `SERVER`)
- Suivi des sessions plugin en temps réel
- Ingestion de données de jeu via WebSocket (namespace `/plugin`)
- Création automatique de matchs depuis les événements plugin
- Lien de lancement Arena Agent copiable

🖼️ Assets & Médias
- Upload fichiers (images, vidéos, audio, documents) — 100 MB max
- Workflow d'approbation `PENDING` / `APPROVED` / `REJECTED`
- Asset packs pour organiser les médias
- URL OBS copiable
- Versioning des assets
- Filtres par événement, catégorie, statut, type, pack

🔔 Notifications
- Types : `FRIEND_REQUEST`, `FRIEND_ACCEPTED`, `GROUP_INVITE`, `EVENT_INVITE`, `SESSION_START`, `SESSION_END`, `MATCH_RESULT`, `SYSTEM`
- Compteur non-lus
- Marquer tout comme lu / archiver
- Action directe depuis la notification (ex : accepter une demande d'ami)

 💬 Messages
- Messagerie intégrée pour événements et groupes

🏢 Organisations (Enterprise)
- Création et gestion d'organisations
- Gestion des membres avec titres

🛡️ Admin & Audit
- Dashboard admin (stats plateforme : users, events, matchs, bans, premium)
- Logs d'audit avec IP, timestamp, métadonnées
- Gestion utilisateurs (ban/unban, plan)

📊 Chiffres clés

| Métrique | Valeur |
|----------|--------|
| Domaines fonctionnels | 28 |
| Routes API | ~120 |
| Namespaces WebSocket | 2 |
| Modèles Prisma | 35+ |

 Statut

Actuellement en développement actif. Beta privée prévue pour le T3 2026.
| Composant | Statut |
|-----------|--------|
| Backend API | ✅ Opérationnel |
| Frontend Web | ✅ Opérationnel |
| Agent Desktop | 🔄 En développement |
| Overlay in-game | 🔄 En développement |
| RSO (Riot Sign-On) | ⏳ **En attente d'approbation** |

À propos du RSO : L'intégration native avec Riot Games (OAuth2 PKCE) a été développée et est techniquement fonctionnelle. Elle est actuellement **en attente de validation par l'équipe Riot Games** avant d'être activée officiellement. En attendant


 📅 Roadmap

- **Actuellement** : Développement actif
- **T3 2026** : Beta privée
- **T4 2026** : Lancement public (sous réserve approbation RSO)

📞 Contact

**Développeur principal** : Bino212@proton.me

---

📄 Licence

Propriétaire — Tous droits réservés © 2026 Arena Hub

---

*Dernière mise à jour : avril 2026*
