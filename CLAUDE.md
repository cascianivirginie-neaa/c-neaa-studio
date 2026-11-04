# Site vitrine NEAA Studio — c-neaa.com

## Projet
Site vitrine statique de NEAA Studio : une seule page `index.html` (HTML + CSS inline, polices Google Fonts).
Baseline : "Studio de logiciels pour les TPE et indépendants — IA & automatisation".
Repo GitHub : cascianivirginie-neaa/c-neaa-studio (branche main).

## Design (validé le 04/11/2026)
- Base blanche + un seul bleu #1D4ED8 ; texte bleu nuit #0B1B3A.
- Touches "noir flashy" uniquement : hero (fond #070B1A + halos bleu/violet/rose), section Méthode (noir uni), bloc CTA final (dégradé bleu > violet > rose), footer noir.
- Titres : Bricolage Grotesque ; texte : Inter.
- Une couleur par produit : Invoxa bleu, Néora violet, Drive Flow cyan, Neaakor rose.

## Code des formes (à respecter partout)
- Arrondi 8px : boutons, badges, icônes (tout ce qui est petit ou cliquable).
- Carré (radius 0) : grands blocs (aperçu hero, référence client, produits, CTA final).
- Trait au-dessus, sans cadre : listes (Expertises, Méthode).

## Contenu
- Sections : hero, bandeau confiance, Services (4), Méthode (4 étapes), Produits, CTA audit gratuit, footer (SIRET, mentions légales).
- Pas de section Réalisations ni de chiffres tant que les projets ne sont pas finis.
- Seul Drive Flow a un lien actif ; Invoxa, Néora, Neaakor = "Bientôt disponible".
- Ne jamais inventer de chiffres ou de témoignages.

## Règles
- Ne jamais publier CERVEAU_*.md ni CONTEXTE_*.md (contexte privé, dans .gitignore).
- Ne jamais utiliser git stash. Pas d'emojis dans le code.
- Toujours préciser le terminal (Claude Code / bash / Hostinger).

## Déploiement
- VPS Hostinger, Caddy en Docker, même modèle que go.c-neaa.com (file_server).
- Ne jamais toucher aux blocs n8n, invoxa, driveflow (port 3000), neora, go.
- Toujours sauvegarder Caddyfile et docker-compose.yml avant modification.
