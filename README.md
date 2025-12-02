# **Velvet Oracle — WebApp Edition**
*Examen d’entrée haut de gamme pour Telegram*

Velvet Oracle WebApp est l’interface officielle permettant de passer l’examen d’entrée Velvet directement **en plein écran dans Telegram**.  
Conçue comme une expérience sobre, immersive et minimaliste, elle prolonge l’esthétique noire-or de Velvet et offre une progression fluide, silencieuse et parfaitement maîtrisée.

---

## ✨ Vision

Velvet Oracle n’est pas un quiz.  
C’est le **seuil d’entrée** d’un cercle où la culture, l’exigence et la maîtrise intérieure trouvent enfin leur place.

Cette WebApp a été pensée comme une porte élégante, une expérience qui parle autant aux sens qu’à l’intellect.

---

## 🎯 Fonctionnalités

- Interface premium **noir-or**, signature Velvet  
- Navigation **plein écran Telegram WebApp**  
- Progression **15 questions** avec transitions fluides  
- **Timer global intégré** (aucune pression, juste une mesure intérieure)  
- Sélection tactile **A/B/C/D** avec animation subtile  
- Narration discrète et équilibrée  
- Envoi automatique des résultats vers le bot Telegram  
- Compatible **TEST / PROD**

---

## 🔗 Intégration Telegram

La WebApp est ouverte via un bouton dédié :

```python
KeyboardButton(
    text="✨ Lancer l’examen Velvet Oracle",
    web_app=WebAppInfo(url="https://velvet-oracle-webapp.vercel.app")
)
