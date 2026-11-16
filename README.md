# Page de sources

Contenu : `_data/site.json`. Page publique : `index.html`. Page de mise à jour : `/admin/`.

## Mise en ligne (toi, une fois)

1. Créer un dépôt public sur GitHub, y déposer tous ces fichiers.
2. Settings > Pages > Source : Deploy from a branch > `main` / `(root)` > Save.
3. URL publique : `https://<utilisateur>.github.io/<depot>/`
4. Ne plus renommer le dépôt après impression du QR code.

## Accès de ta copine à la page de mise à jour

1. GitHub > Settings > Developer settings > Personal access tokens > Fine-grained tokens > Generate new token.
2. Repository access : Only select repositories > le dépôt de la page.
3. Permissions > Repository permissions > Contents : Read and write. Rien d'autre.
4. Expiration : la plus longue proposée.
5. Lui envoyer en privé ce lien (une seule fois) :
   `https://<utilisateur>.github.io/<depot>/admin/#t=<JETON>`
6. Le jeton est mémorisé dans son navigateur et retiré de l'adresse. Ensuite elle utilise `/admin/` (à mettre en favori).

Le jeton donne un accès en écriture à ce seul dépôt : ne pas le publier. En cas de fuite ou d'expiration, le révoquer ou le régénérer dans GitHub et renvoyer un nouveau lien.

## Utilisation (elle)

- Ouvrir `/admin/`, modifier titre, sections, sources, liens.
- Enregistrer. La page publique se met à jour en 1 à 2 minutes.
- Italique : `*texte*`, gras : `**texte**`.

## Secours

Le contenu reste modifiable à la main sur github.com : `_data/site.json` > crayon > Commit changes.
