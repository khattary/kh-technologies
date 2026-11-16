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

## À compléter : les coordonnées

La rubrique Contact affiche « Coordonnées en cours de publication ». Dans `index.html`, chercher
`coords-pending` et remplacer le paragraphe par ce bloc, en gardant seulement les lignes utiles :

```html
<ul class="coords">
  <li><span>E-mail</span><a href="mailto:contact@exemple.mr">contact@exemple.mr</a></li>
  <li><span>Téléphone</span><a href="tel:+22200000000">+222 00 00 00 00</a></li>
  <li><span>Adresse</span><b>Adresse postale, Nouakchott</b></li>
  <li><span>LinkedIn</span><a href="https://www.linkedin.com/company/exemple" rel="noopener">linkedin.com/company/exemple</a></li>
</ul>
```

Les valeurs ci-dessus sont des exemples de forme, pas des coordonnées réelles.

## Nom de domaine

L'hébergement est gratuit. Un nom de domaine propre (`.mr`, `.com`) est payant, à l'année, chez un bureau
d'enregistrement. GitHub Pages accepte un domaine personnalisé et fournit le certificat HTTPS sans frais :
dans le dépôt, Settings → Pages → Custom domain. Il faudra alors remplacer l'adresse
`https://khattary.github.io/kh-technologies/` dans `index.html`, `sitemap.xml` et `robots.txt`.

## Polices

Montserrat et Inter sont chargées depuis Google Fonts. Pour ne dépendre d'aucun service tiers,
elles peuvent être hébergées avec le site.
