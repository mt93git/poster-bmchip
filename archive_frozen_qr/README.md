# ⚠️ CONTRAT D'IMMUTABILITÉ DU QR CODE — BM-CHIP C2-LOEX
## REGISTRE DE GOUVERNANCE SCIENTIFIQUE ET TECHNIQUE POUR COLLABORATEURS ET SUCCESSEURS
**Projet :** Jumeau Numérique 3D & Modélisation Biophysique BM-Chip (Organe-sur-Puce Médullaire)  
**Laboratoire :** Laboratoire d'Organogénèse Expérimentale (LOEX), Centre de Recherche du CHU de Québec, Université Laval  
**Date de Gel Formel :** 14 Octobre 2026  
**Événement de Soumission :** Soumission officielle du Poster Scientifique (TheCell 2026 / LOEX)  
**Auteur Principal & Architecte :** Maxime Tricaud (PhD Cand. Yale University / LOEX Université Laval)  

---

> [!CAUTION]
> ### 🛑 AVERTISSEMENT CRITIQUE — NE JAMAIS MODIFIER OU SUPPRIMER CETTE URL
> Le QR code associé à ce document est **DÉFINITIVEMENT IMPRIMÉ ET GRAVÉ** sur le poster scientifique soumis.  
> Une fois le poster imprimé et soumis, **ce QR code ne peut plus être modifié physiquement**.  
> Tout changement, déplacement, renommage de dépôt ou rupture de redirection brisera l'accès pour tous les lecteurs, évaluateurs et conférenciers scannant le poster physique.

---

### 1. Le Principe Fondamental : Découplage Contenant / Contenu

Dans ce projet, le QR Code et son URL constituent le **Contenant Immuable (Adresse Web Permanente)**, tandis que l'application Web 3D constitue le **Contenu Évolutif** :

$$\underbrace{\text{QR Code Physique } \longrightarrow \text{ URL Canonique}}_{\textbf{IMMUTABLE À PERPÉTUITÉ}} \quad \Longrightarrow \quad \underbrace{\text{Code WebGL, Physique, Télémétrie}}_{\textbf{LIBREMENT MODIFIABLE EN CONTINU}}$$

1. **Ce qui est IMMUTABLE (Ne jamais toucher) :**
   - Le QR Code gravé sur le poster.
   - L'URL cible directe : `https://mt93git.github.io/poster-bmchip/viewer3d.html#tab=qr`
   - L'URL passerelle racine : `https://mt93git.github.io/poster-bmchip/`
   - Le compte GitHub : `mt93git`
   - Le nom du dépôt : `poster-bmchip`
   - La branche déployée : `main` (hébergement GitHub Pages)

2. **Ce qui est LIBREMENT MODIFIABLE (Faites évoluer le code !) :**
   - L'interface 3D dans [`viewer3d.html`](viewer3d.html) (rendus, textures, géométrie de la puce, vitesse d'affichage, graphiques).
   - Les modèles physiques, les équations analytiques et les cinétiques d'oxygène.
   - Les palettes de couleurs et styles CSS.
   - Le comportement du routeur dynamique dans [`index.html`](index.html) et [`config.json`](config.json).

---

### 2. Les 3 Règles d'Or pour les Futurs Développeurs et Collaborateurs

#### Règle 1 : Préservation de l'Arborescence et des Noms de Fichiers
- **NE JAMAIS** renommer `viewer3d.html` (ex: ne pas le changer en `viewer_v2.html` ou `app.html`).
- **NE JAMAIS** déplacer `viewer3d.html` dans un sous-dossier sans laisser un fichier miroir ou une redirection automatique.
- Toute mise à jour de l'application 3D doit écraser ou enrichir directement `viewer3d.html`.

#### Règle 2 : Maintien de GitHub Pages sur la Branche `main`
- Le dépôt doit impérativement conserver GitHub Pages activé avec pour source la racine `/` de la branche `main`.
- La présence du fichier vide `.nojekyll` à la racine est obligatoire pour éviter que GitHub Pages n'ignore les fichiers avec soulignés ou certains modules.

#### Règle 3 : Protocole de Migration ou de Redirection Institutionnelle
Si à l'avenir l'Université Laval ou le LOEX héberge cette application sur un serveur dédié ou un nom de domaine institutionnel (ex: `https://bmchip.loex.ulaval.ca/`), **le dépôt GitHub actuel doit rester actif** :
- Soit en mettant à jour [`config.json`](config.json) avec la nouvelle cible (`"target_url": "https://bmchip.loex.ulaval.ca/"`).
- Soit en conservant un `viewer3d.html` qui charge ou redirige vers le nouveau serveur.
- **En aucun cas le dépôt d'origine ne doit renvoyer une erreur 404.**

---

### 3. Actifs Gelés et Empreintes Cryptographiques (SHA-256)

Les fichiers suivants sont certifiés, vérifiés par décodage machine univoque (OpenCV / pyzbar), et archivés pour l'intégration dans le poster :

| Fichier | Format & Spécification | Cible Encodée | Empreinte SHA-256 |
| :--- | :--- | :--- | :--- |
| **`CANONICAL_QR_DIRECT_VECTOR.svg`** | Vectoriel SVG pur (résolution infinie) | `https://mt93git.github.io/poster-bmchip/viewer3d.html#tab=qr` | `fe9c3b5dc8610866913b317a11cad5de9adfbc4c2ecb648fe0d2055f9e573c2a` |
| **`CANONICAL_QR_DIRECT_MATRIX_300DPI.png`** | Matrice carrée 300 DPI sans texte | `https://mt93git.github.io/poster-bmchip/viewer3d.html#tab=qr` | `b0fc688c1e734936b22cf9f8dc61d1e0f3d3d4008f716e94811cc85f2e964c50` |
| **`CANONICAL_QR_DIRECT_WITH_LEGEND.png`** | Carte 300 DPI avec cartouche & URL | `https://mt93git.github.io/poster-bmchip/viewer3d.html#tab=qr` | `ae6c4de25ab40f68ff0d295063d850c1caec6b626526dbab058fa163a26d23ac` |
| **`CANONICAL_QR_ROOT_PORTAL_MATRIX_300DPI.png`** | Matrice 300 DPI passerelle dynamique | `https://mt93git.github.io/poster-bmchip/` | `65de7383dac27be31a389d1981d8dba992bd6a2c7be9da2f0bf2dbeebb8e290f` |

- **Niveau de tolérance aux pannes :** `Level Q` (Quartile — capacité de correction d'erreurs jusqu'à **25%**).  
  Même en cas de rayure, de plis de transport sur le tissu du poster, de reflets sous les néons du palais des congrès ou de légère salissure, le QR code restera 100% décodable par les caméras mobiles.

---

### 4. Quel QR Code intégrer dans le poster ?

1. **Recommandation optimale :**  
   Utiliser **`CANONICAL_QR_DIRECT_VECTOR.svg`** (ou **`CANONICAL_QR_DIRECT_MATRIX_300DPI.png`**).  
   Ces deux fichiers encodent directement l'URL d'atterrissage du jumeau :  
   `https://mt93git.github.io/poster-bmchip/viewer3d.html#tab=qr`  
   L'expérience utilisateur est immédiate, sans aucun temps de chargement intermédiaire.

2. **Alternative passerelle dynamique :**  
   Si le poster utilise déjà le QR code `https://mt93git.github.io/poster-bmchip/`, **celui-ci est également 100% opérationnel** et redirige instantanément vers le jumeau via `index.html` et `config.json`.

---

### 5. Lieux d'Archivage Pérenne

Ce dossier d'archives et cette notice sont répliqués de manière identique dans trois environnements de travail :

1. **Dossier du Poster TheCell 2026 :**  
   `Univ_Paper/03_Academics_and_Courses/03_Seminars_and_Conferences/TheCell_2026_Poster_Master_Dossier/assets/00_FROZEN_CANONICAL_QR_CODE/`
2. **Plateforme de Modélisation LOEX (Research Hub) :**  
   `Lab_Domains/04_Modelization/post-claude-review_2026_10_07/chamber_viewer/00_FROZEN_CANONICAL_QR_CODE/`
3. **Dépôt Git Public Déployé :**  
   `poster-bmchip/archive_frozen_qr/` (visible sur GitHub par toute personne clonant le code)

*Fait à Québec / LOEX Université Laval, le 14 octobre 2026.*
