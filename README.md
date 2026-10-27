# ERP Pro - Site Vitrine

Site vitrine moderne pour **ERP Pro**, une solution de gestion d'entreprise (ERP) conçue spécifiquement pour les entreprises africaines. Le site présente les fonctionnalités du produit et permet de demander des démonstrations.

## 🎯 Aperçu du Projet

ERP Pro est une plateforme de gestion multi-sites qui permet de piloter :
- **Ventes et caisse**
- **Gestion des stocks**
- **Achats et fournisseurs**
- **Comptabilité**
- **Gestion des employés et clients**
- **Rapports et statistiques**
- **Synchronisation hors-ligne** (adaptée aux connexions instables)

## 📁 Structure du Projet

```
ERP/
├── index.html              # Page d'accueil (hero, sections principales)
├── fonctionnalites.html    # Page détaillant les 10 fonctionnalités
├── style.css               # Styles communs (couleurs, boutons, composants)
├── home.css                # Styles spécifiques à l'accueil (hero, bento, carrousel)
├── hero-bg.mp4             # Vidéo 3D de fond du hero
├── hero-poster.jpg         # Image de poster pour la vidéo
├── fondateur.jpg           # Photo de la section "À propos"
└── README.md               # Ce fichier
```

## 🚀 Installation et Utilisation

### Prérequis
- Aucun prérequis particulier : le site est en HTML/CSS/JS pur
- Navigateur moderne compatible avec les fonctionnalités ES6+

### Démarrage Local

1. Clonez ou téléchargez le dossier du projet
2. Ouvrez simplement `index.html` dans votre navigateur

```bash
# Sur Windows (avec Git Bash ou PowerShell)
start index.html

# Sur macOS
open index.html

# Sur Linux
xdg-open index.html
```

### Déploiement

Le site peut être déployé sur n'importe quel hébergement statique :
- GitHub Pages
- Netlify
- Vercel
- Serveur web traditionnel (Apache, Nginx)

## 🎨 Design et Technologies

### Polices
- **Bricolage Grotesque** (titres) - Google Fonts
- **Plus Jakarta Sans** (texte) - Google Fonts

### Caractéristiques
- Design responsive (mobile-first)
- Animations au défilement (Intersection Observer)
- Navigation flottante avec effet de transparence
- Menu mobile hamburger
- Palette de couleurs teal/mint (#0F8F82, #22C7B5, #E6F6F3)
- Icônes SVG intégrées

### JavaScript
- Scripts légers sans dépendances externes
- Génération dynamique des fonctionnalités dans `fonctionnalites.html`
- Animations au défilement
- Menu mobile et navigation sticky

## 📝 Modification du Contenu

### Modifier les textes

Dans **index.html** :
- Recherchez le texte avec `Ctrl+F` pour le modifier
- Cherchez les commentaires `<!-- SECTION : ... -->` pour naviguer rapidement
- Les sections sont dans l'ordre d'affichage

Dans **fonctionnalites.html** :
- Les fonctionnalités sont générées par JavaScript (lignes 126-147)
- Modifiez la liste `F` pour changer les textes, descriptions ou illustrations
- Chaque entrée contient : `id`, `t` (titre), `p` (icône SVG), `d` (description), `l` (liste), `i` (illustration)

### Modifier les couleurs

Les couleurs sont définies comme variables CSS dans **style.css** :
- `--p` : couleur principale (teal)
- `--ac` : couleur accentuée
- `--bg` : couleur de fond
- `--tx` : couleur du texte
- etc.

### Ajouter une fonctionnalité

Dans `fonctionnalites.html`, ajoutez une entrée à la liste `F` :

```javascript
{id:'nouvelle-fonction',t:'Titre de la fonction',p:'chemin-svg',d:'Description courte',l:['Point 1','Point 2','Point 3'],i:'code-html-illustration'}
```

### Modifier le numéro WhatsApp

Le lien WhatsApp est présent dans :
- `index.html` (ligne 79) : lien de la démo dans le hero
- `fonctionnalites.html` (ligne 93) : lien de la démo final

Modifiez le numéro dans l'URL : `https://wa.me/22892877153?text=...`

## 📱 Pages

### Page d'accueil (`index.html`)
- **Hero** : Titre principal avec vidéo 3D de fond et maquette du dashboard
- **Simplifiez la gestion** : 3 cartes + dashboard incliné
- **Fonctionnalités** : Grille bento (5 cartes)
- **Secteurs** : Carrousel des industries ciblées
- **À propos** : Section avec photo du fondateur
- **FAQ** : Questions fréquentes
- **Contact** : CTA final pour demander une démo

### Page Fonctionnalités (`fonctionnalites.html`)
- En-tête avec pastilles de navigation
- 10 blocs détaillant chaque module :
  1. Gestion multi-sites
  2. Gestion des stocks
  3. Ventes et caisse
  4. Achats et fournisseurs
  5. Statistiques et rapports
  6. Comptabilité
  7. Gestion des employés
  8. Gestion des clients
  9. Bons et documents
  10. Synchronisation hors-ligne

## 🎯 Points d'Intégration

### Lien WhatsApp
- Numéro actuel : +228 92 87 71 53
- Message pré-rempli pour la demande de démo

### Email de contact
- gbadamassia@gmail.com

## 🔧 Personnalisation Avancée

### Changer la vidéo du hero
1. Remplacez `hero-bg.mp4` par votre vidéo
2. Mettez à jour `hero-poster.jpg` avec l'image de poster correspondante
3. Assurez-vous que la vidéo est en format MP4 pour la compatibilité

### Modifier les icônes SVG
Les icônes sont intégrées directement dans le HTML. Pour les modifier :
- Les chemins SVG sont dans les attributs `d` des balises `<path>`
- Utilisez un éditeur SVG (Figma, Illustrator) pour créer de nouvelles icônes
- Copiez le chemin `d` et remplacez l'existant

### Ajuster les animations
- Les animations au défilement utilisent `IntersectionObserver`
- La classe `.vis` est ajoutée quand un élément entre dans la vue
- Modifiez les transitions CSS dans `style.css` pour ajuster la durée et l'effet

## 📊 Navigation

### Navigation principale
- Produit
- Fonctionnalités (redirige vers `fonctionnalites.html`)
- Secteurs
- À propos
- FAQ
- Contact

### Menu mobile
- S'ouvre avec le bouton hamburger
- Liens identiques à la navigation desktop
- Animation fluide d'ouverture/fermeture

## 🌐 Compatibilité

- **Navigateurs** : Chrome, Firefox, Safari, Edge (versions récentes)
- **Mobile** : iOS Safari, Chrome Mobile
- **Desktop** : Windows, macOS, Linux
- **Accessibilité** : ARIA labels, navigation au clavier, contrastes respectés

## 📄 Licence

© 2026 ERP Pro. Tous droits réservés.

## 🤝 Support

Pour toute question ou demande de démonstration :
- **WhatsApp** : +228 92 87 71 53
- **Email** : gbadamassia@gmail.com

---

**Développé avec ❤️ pour les entreprises africaines**
