 AfricaArt
Présentation du projet
AfricaArt est une application hybride (Ionic + Angular) qui facilite l’achat – et bientôt la location – de tenues africaines pour femmes, hommes et enfants. Le projet valorise l’habillement « tradi-moderne » sénégalais ; il mêle authenticité culturelle et expérience d’achat mobile moderne. 

Fonctionnalités principales
Module	Détails
On-boarding	Écran de bienvenue avec slides automatiques, connexion / inscription avec validations de formulaire. 
Accueil	Logo + message d’accueil, barre de recherche, catégories, mise en avant des 4 meilleures tenues, footer (Home / Favoris / Profil). 
Catalogue & Favoris	Liste des articles, filtre par catégorie, ajout / retrait des favoris.
Fiche produit	Galerie d’images, prix, description courte, bouton « Réserver » (redirection vers Google Forms). 
Profil utilisateur	Infos personnelles, historique de réservations (à venir).
Back-office à venir	Gestion des stocks, commandes et statistiques.

Stack & architecture
Framework : Ionic 6 + Angular 17

Langages : TypeScript, HTML 5, CSS 3

Outils runtime : Node ≥ 18, npm, Ionic CLI, Capacitor/Cordova pour la couche native 

Design tokens : palette marron / beige / orange / jaune / blanc + police Arial (charte graphique interne). 

Prérequis
bash
Copier
Modifier
# Node, npm et Ionic CLI
node -v        # ≥ 18.x
npm  -v        # ≥ 10.x
npm install -g @ionic/cli cordova
Installation rapide
bash
Copier
Modifier
# 1. Cloner le dépôt
git clone https://github.com/<org>/africaart.git
cd africaart

# 2. Installer les dépendances
npm ci

# 3. Lancer l’app en mode web / PWA
ionic serve       # http://localhost:8100
Builds mobiles
bash
Copier
Modifier
# Android debug
ionic cap add android
ionic cap run android -l --external

# iOS (macOS uniquement)
ionic cap add ios
ionic cap run ios -l --external
Organisation du dépôt
text
Copier
Modifier
src/
 ├── app/            # modules Angular & pages Ionic
 ├── assets/         # images, icônes, charte graphique
 ├── environments/   # configs dev / prod
 └── theme/          # variables CSS & Tailwind (optionnel)
Roadmap (extraits du business plan)
Location de tenues pour écoles & événements culturels

Intégration d’un paiement mobile (Orange Money / Wave)

Tableau de bord analytique pour les vendeurs

Internationalisation FR/EN/Wolof 

Contribuer
Fork, créez votre branche (git checkout -b feature/ma-feature)

Commitez vos changements (git commit -m "Feat: …")

Poussez la branche (git push origin feature/ma-feature)

Ouvrez une Pull Request – nous suivons Conventional Commits + semantic versioning.

Auteurs
Tamsir Ndiaye – Lead dev & assistant projet

Awa Fall – Lead dev & gestion produit


« S’habiller, c’est plus qu’un besoin : c’est affirmer son identité. »
AfricaArt – Un peuple, un but, une foi.
