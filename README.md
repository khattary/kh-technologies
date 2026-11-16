# Site institutionnel KH TECHNOLOGIES

Site statique d'une seule page : tout est dans `index.html` (styles, scripts et pictogrammes intégrés).
Aucune base de données, aucun serveur applicatif, aucune dépendance à installer.

## Contenu du dossier

| Fichier | Rôle |
|---|---|
| `index.html` | Le site |
| `404.html` | Page affichée pour une adresse inconnue |
| `favicon.ico`, `favicon.svg`, `apple-touch-icon.png`, `icon-192.png`, `icon-512.png` | Icônes du site |
| `og-image.png` | Image affichée lors d'un partage (LinkedIn, WhatsApp) |
| `site.webmanifest`, `robots.txt`, `.nojekyll` | Fichiers techniques pour les navigateurs, les moteurs de recherche et GitHub Pages |

## Avant la mise en ligne : les coordonnées

La rubrique Contact affiche « Coordonnées en cours de publication ». Dans `index.html`, cherchez
`coords-pending` et remplacez le paragraphe par ce bloc, en gardant seulement les lignes utiles :

```html
<ul class="coords">
  <li><span>E-mail</span><a href="mailto:contact@exemple.mr">contact@exemple.mr</a></li>
  <li><span>Téléphone</span><a href="tel:+22200000000">+222 00 00 00 00</a></li>
  <li><span>Adresse</span><b>Adresse postale, Nouakchott</b></li>
  <li><span>LinkedIn</span><a href="https://www.linkedin.com/company/exemple" rel="noopener">linkedin.com/company/exemple</a></li>
</ul>
```

Les valeurs ci-dessus sont des exemples de forme, pas des coordonnées réelles.

## Mise en ligne gratuite

### Option A — GitHub Pages

1. Créer un dépôt public sur github.com, par exemple `kh-technologies`.
2. Y déposer tout le contenu de ce dossier (bouton « Add file → Upload files », ou `git push`).
3. Dans le dépôt : Settings → Pages → Source « Deploy from a branch », branche `main`, dossier `/ (root)`, puis Save.
4. Le site est en ligne après une à deux minutes à l'adresse `https://<identifiant>.github.io/kh-technologies/`.

### Option B — Netlify ou Cloudflare Pages

Créer un compte gratuit, choisir le déploiement par dépôt de fichiers (« Deploy manually » chez Netlify,
« Upload assets » chez Cloudflare Pages) et y glisser ce dossier. L'adresse est fournie aussitôt.

## Après la mise en ligne

- **Image de partage.** Dans `index.html`, remplacer `content="og-image.png"` par l'adresse complète,
  par exemple `https://<adresse-du-site>/og-image.png` : les réseaux sociaux exigent une adresse absolue.
- **Nom de domaine.** L'hébergement est gratuit ; un nom de domaine propre (`.mr`, `.com`) est payant,
  à l'année, chez un bureau d'enregistrement. Les trois hébergeurs ci-dessus acceptent un domaine personnalisé
  et fournissent le certificat HTTPS sans frais.
- **Polices.** Montserrat et Inter sont chargées depuis Google Fonts. Pour ne dépendre d'aucun service tiers,
  elles peuvent être hébergées avec le site.
