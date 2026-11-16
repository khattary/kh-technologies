# Site institutionnel KH TECHNOLOGIES

Site en ligne : https://khattary.github.io/kh-technologies/

Site statique d'une seule page : tout est dans `index.html` (styles, scripts et pictogrammes intégrés).
Aucune base de données, aucun serveur applicatif, aucune dépendance à installer.

## Hébergement

Le site est hébergé gratuitement par GitHub Pages, depuis la branche `gh-pages` de ce dépôt.
La branche `main` contient les mêmes fichiers et sert de référence.

Pour publier une modification, envoyer les fichiers sur `gh-pages` (et sur `main`) :

```bash
git add -A
git commit -m "Mise à jour du site"
git push origin main
git push origin main:gh-pages
```

La mise à jour est visible après une à deux minutes.

## Contenu

| Fichier | Rôle |
|---|---|
| `index.html` | Le site |
| `404.html` | Page affichée pour une adresse inconnue |
| `favicon.ico`, `favicon.svg`, `apple-touch-icon.png`, `icon-192.png`, `icon-512.png` | Icônes du site |
| `og-image.png` | Image affichée lors d'un partage (LinkedIn, WhatsApp) |
| `sitemap.xml`, `robots.txt` | Indications pour les moteurs de recherche |
| `site.webmanifest`, `.nojekyll` | Fichiers techniques pour les navigateurs et GitHub Pages |

## Modifier les coordonnées

Les coordonnées de la rubrique Contact se trouvent dans `index.html`, dans la liste `<ul class="coords">` :
une ligne `<li>` par coordonnée (e-mail, téléphone, WhatsApp, adresse). Le lien WhatsApp a la forme
`https://wa.me/` suivi du numéro complet, sans `+` ni espace. Les mêmes e-mail et téléphone figurent aussi
dans le bloc `application/ld+json` en tête de fichier, lu par les moteurs de recherche.

## Nom de domaine

L'hébergement est gratuit. Un nom de domaine propre (`.mr`, `.com`) est payant, à l'année, chez un bureau
d'enregistrement. GitHub Pages accepte un domaine personnalisé et fournit le certificat HTTPS sans frais :
dans le dépôt, Settings → Pages → Custom domain. Il faudra alors remplacer l'adresse
`https://khattary.github.io/kh-technologies/` dans `index.html`, `sitemap.xml` et `robots.txt`.

## Polices

Montserrat et Inter sont chargées depuis Google Fonts. Pour ne dépendre d'aucun service tiers,
elles peuvent être hébergées avec le site.
