# 🐺 Créer une Chasse aux Questions (avec GitHub Pages + QR Codes)

Bienvenue ! Ce projet permet de créer un petit jeu où les gens scannent des QR codes pour répondre à des questions. Chaque QR code ouvre une question différente sur un site web.

Pas besoin d’être développeur ! Voici comment ça marche 👇

---

## 🔗 1. Le site

Ce projet est hébergé ici :
👉 **https://demoparcalpha.github.io/qr-quiz/**

Chaque question est visible à une adresse comme :
👉 `https://demoparcalpha.github.io/qr-quiz/?id=1`
👉 `https://demoparcalpha.github.io/qr-quiz/?id=2`
👉 etc.

---

## 📁 2. Où sont les questions ?

Elles sont dans un fichier appelé `contenus.json`.
Ce fichier contient toutes les questions du jeu.

### Exemple de question dans `contenus.json` :

```json
"1": {
    "title": "Quelle est la principale source de nourriture du loup gris ?",
    "subtitle": "Question nourriture",
    "answers": [
      "🍓 Fruits et baies",
      "🦌 Grands herbivores",
      "🐟 Poissons"
    ],
    "answer": 1,
    "image": "https://i.imgur.com/hVviAl2.jpg"
}
```
### Pages sans question :
Il est possible de faire une page sans questions en laissant `answers` vide :
```json
    "answers": [],
```
Ou en supprimant la ligne.

### Exemple de page sans question :
Voici un exemple concret d'une page de bienvenue
```json
"0": {
    "title": "Bienvenue, on va faire un ptit quiz !",
    "subtitle": "Trouve tous les QR codes et réponds aux questions. Bonne chasse !",
    "answers": [],
    "answer": 0,
    "image": "https://i.pinimg.com/736x/7a/be/1a/7abe1abf3070503422825065bcf62b47.jpg"
}
```