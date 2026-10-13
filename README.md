# 🛰️ BM-Chip C2-LOEX : Portail d'Accès Dynamique Poster & Jumeau Numérique

Portail de redirection souverain pour les posters scientifiques présentés en congrès internationaux par l'équipe du LOEX (Centre de Recherche du CHU de Québec - Université Laval).

---

## 📱 URL Canonique Immuable (Imprimée sur le Poster)

👉 **https://mt93git.github.io/poster-bmchip/**

Cette URL est gravée sur le QR Code du poster imprimé. Elle ne changera **jamais**.

---

## 🎛️ Mode d'Emploi : Piloter l'accès en 3 secondes depuis GitHub

Pour modifier la redirection ou couper l'accès, il vous suffit d'éditer le fichier [`config.json`](config.json) directement sur GitHub :

### 1. Activer / Couper l'accès (Kill-Switch)
- **Accès Ouvert (Pendant le congrès) :**
  ```json
  "status": "ON"
  ```
  *Le visiteur scannant le QR code est redirigé immédiatement vers le jumeau numérique 3D.*

- **Accès Fermé (Après le congrès / Protection de la PI) :**
  ```json
  "status": "OFF"
  ```
  *Le visiteur voit une page sobre annonçant la clôture de la session avec vos coordonnées universitaires pour demander un tiré-à-part ou un accès privilégié.*

---

### 2. Changer la Cible de Redirection (`target_url`)
Vous pouvez pointer vers n'importe quelle ressource :
- **`viewer3d.html`** *(Par défaut)* : Le jumeau numérique autonome 3D hébergé directement sur GitHub (fonctionne 24h/24 sans nécessiter d'ordinateur allumé).
- **`https://votre-tunnel-cloudflare.com/#tab=qr`** : Un serveur de simulation temps-réel connecté à votre banc expérimental lors d'une démonstration en direct.
- **`https://drive.google.com/...`** : Un PDF haute définition du poster ou un article sous presse.

---

## 🏛️ Traçabilité
- **Laboratoire :** LOEX / Université Laval / CHU de Québec
- **Projet :** BM-Chip C2-LOEX (Niche Médullaire Vasculaire & Endotéliale)
- **Auteur :** Maxime Tricaud
