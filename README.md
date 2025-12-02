# velvet-oracle-webapp
Velvet Oracle WebApp est l’interface officielle permettant de passer l’examen d’entrée Velvet directement en plein écran dans Telegram.

Velvet Oracle — WebApp Edition

Examen d’entrée haut de gamme pour Telegram

Velvet Oracle WebApp est l’interface officielle permettant de passer l’examen d’entrée Velvet directement en plein écran dans Telegram.
Conçue comme une expérience sobre, immersive et minimaliste, elle prolonge l’esthétique noire-or de Velvet et offre une progression fluide, silencieuse et parfaitement maîtrisée.

✨ Vision

Velvet Oracle n’est pas un quiz.
C’est le seuil d’entrée d’un cercle où la culture, l’exigence et la maîtrise intérieure retrouvent leur place.

Cette WebApp a été pensée pour devenir la porte élégante qui précède l’admission : une expérience qui parle autant aux sens qu’à l’intellect.

🎯 Fonctionnalités

Interface premium noir-or, inspirée de l’univers Velvet

Navigation plein écran Telegram WebApp

Progression 1 → 15 avec transitions fluides

Timer total intégré (aucune pression, seulement une mesure intérieure)

Sélection tactile A/B/C/D avec animation discrète

Narration subtile pour accompagner chaque question

Envoi automatique du résultat au bot Telegram

Compatible PROD/TEST via le bot

🔗 Intégration Telegram

La WebApp est lancée via un bouton dédié dans le bot Velvet Oracle :

KeyboardButton(
    text="✨ Lancer l’examen Velvet Oracle",
    web_app=WebAppInfo(url="https://velvet-oracle-webapp.vercel.app")
)


Une fois l’examen complété, la WebApp transmet au bot un JSON structuré :

{
  "mode": "exam_v1",
  "score": 13,
  "total": 15,
  "total_time_seconds": 87,
  "answers": [
    { "question_id": 1, "status": "correct", "choice_letter": "B" }
  ]
}


Le bot :

calcule le profil cognitif du joueur

vérifie la tentative unique en mode PROD

consigne l’examen dans Notion

renvoie le verdict Admis / Porte encore close

🧠 Architecture

Front : HTML5 / CSS3 (design Velvet)

Script : JavaScript vanilla

Bridge : Telegram WebApp JS SDK

Backend : géré par le bot Python (python-telegram-bot 20.x)

Database : Notion API (Velvet Oracle — Examens)

Hébergement : Vercel (static site, haute performance)

📦 Contenu du repository

index.html — Core de la WebApp

/assets (optionnel) — images, icônes, backgrounds

Documentation d’intégration Telegram (en cours)

🚀 Déploiement (Vercel)

Connecter le repository GitHub à Vercel

Framework preset : Static

Build command : (vide)

Output directory : .

Déployer

Vercel génère une URL HTTPS, compatible Telegram.

🕯 Héritage Velvet

Chaque détail de cette WebApp porte la signature Velvet :
silence, élégance, précision.
Une passerelle entre toi et ceux qui reconnaissent la beauté d’une épreuve bien conçue.

Velvet Oracle — Love with Impact. Culture with Presence.
