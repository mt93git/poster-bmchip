# 🛰️ BM-Chip C2-LOEX : Portail d'Accès Dynamique Poster & Jumeau Numérique

Portail de redirection souverain pour les posters scientifiques présentés en congrès internationaux par l'équipe du LOEX (Centre de Recherche du CHU de Québec - Université Laval).

---

## 📱 URLs Canoniques Immuables (Gravées sur les Posters)

1. **URL Directe Jumeau 3D (Recommandée Poster) :**
   👉 **https://mt93git.github.io/poster-bmchip/viewer3d.html#tab=qr**
   *(Charge directement le jumeau numérique 3D en mode Jour, volet masqué par défaut, vitesse x500).*

2. **URL Passerelle Racine (Portail dynamique & Kill-Switch) :**
   👉 **https://mt93git.github.io/poster-bmchip/**
   *(Redirige instantanément vers le jumeau 3D ou affiche la page de veille selon `config.json`).*

> [!IMPORTANT]
> **CONTRAT D'IMMUTABILITÉ (WORM) :** Ces deux URLs et les fichiers QR correspondants archivés dans [`archive_frozen_qr/`](archive_frozen_qr/) sont **définitivement gelés**. Ne jamais renommer ce dépôt, ne jamais désactiver GitHub Pages, et ne jamais supprimer `viewer3d.html`. Seul le code interne peut être mis à jour. Voir la notice complète dans [`archive_frozen_qr/README.md`](archive_frozen_qr/README.md).

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
