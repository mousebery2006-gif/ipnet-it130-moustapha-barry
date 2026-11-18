# ipnet-it130 - Mon Blog

Travaux pratiques du cours **IT 130 - Introduction aux Technologies Web**.
Ce dépôt regroupe les pages réalisées durant les trois premières semaines :
une page d'accueil, un blog et une page de contact (Semaine 3).

## Contenu du dépôt

| Fichier        | Description                          |
|----------------|--------------------------------------|
| `index.html`   | Page d'accueil (Semaine 1)           |
| `blog.html`    | Page de blog (Semaine 2)             |
| `contact.html` | Page de contact (Semaine 3)          |
| `style.css`    | Feuille de style commune             |
| `README.md`    | Description du projet                |

## Prévisualiser le site en local

Avec VS Code, utiliser l'extension **Live Server**, ou lancer un serveur local :

```bash
python -m http.server 8000
```

Puis ouvrir <http://localhost:8000/> dans le navigateur.

## Publication sur GitHub Pages

Le site est publié à l'adresse suivante :

<https://votre-nom.github.io/ipnet-it130-prenom-nom/>

La page de contact est accessible directement ici :

<https://votre-nom.github.io/ipnet-it130-prenom-nom/contact.html>

> Remplacer `votre-nom` et `prenom-nom` par les valeurs réelles du dépôt GitHub.

## Vérifications effectuées (TP Semaine 3)

Tests de la validation native du formulaire (Chromium) :

| Test | Résultat observé | Conforme |
|------|------------------|----------|
| Champs vides | « Veuillez renseigner ce champ. » sur le nom | Oui |
| Email invalide (`abc`) | « Veuillez inclure "@" dans l'adresse e-mail. » | Oui |
| Message < 10 caractères | « Veuillez allonger ce texte pour qu'il comporte au moins 10 caractères. » | Oui |
| Case RGPD non cochée | « Veuillez cocher cette case si vous souhaitez continuer. » | Oui |
| Formulaire valide | Soumission autorisée | Oui |

Contrôles d'accessibilité :

- Chaque champ a un `<label>` associé via `for`/`id`.
- Un seul `<h1>` par page, hiérarchie des titres respectée (`h1` > `h2` > `h3`).
- Tableaux avec `<caption>`, `<thead>`/`<tbody>`/`<tfoot>` et `<th scope="col|row">`.
- Vidéo et audio avec contrôles et texte de repli (MP4/WebM, MP3/OGG).
- Navigation au clavier avec focus visible (contour de 3 px).
- Contrastes de texte conformes WCAG AA (≥ 4,5:1).

> Les médias de démonstration sont chargés depuis W3Schools et nécessitent
> une connexion Internet.
