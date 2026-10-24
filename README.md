# Mottelo — pages légales et conformité Google Play

Ce dépôt contient des pages statiques à publier avec GitHub Pages :
- `index.html` : page d'accueil et liens légaux
- `privacy-policy.html` : politique de confidentialité
- `data-safety.html` : aide-mémoire public sur les données et la déclaration Google Play
- `terms.html` : conditions générales d'utilisation
- `account-deletion.html` : instructions de suppression du compte et des données

## Avant publication — obligatoire

1. Remplacez tous les champs `À COMPLÉTER` (éditeur, contact, URL, date, juridiction).
2. Vérifiez que chaque déclaration correspond au code réellement publié et à la configuration Supabase.
3. Vérifiez les données réellement envoyées à des tiers (Supabase, Google Play Billing, publicité/analytics s'il y en a).
4. La page `data-safety.html` est une page d'information destinée aux utilisateurs ; elle ne remplace PAS le formulaire « Sécurité des données » dans Play Console.
5. Testez la suppression du compte de bout en bout. La suppression doit effectivement supprimer ou anonymiser les données liées, y compris les sauvegardes et données détenues par des prestataires selon leurs délais.
6. Publiez ces pages via GitHub Pages et fournissez les URL publiques dans Play Console.

## Publier avec GitHub Pages

1. Créez un dépôt GitHub public nommé par exemple `mottelo-legal`.
2. Décompressez ce ZIP et envoyez tous les fichiers à la racine du dépôt.
3. Dans **Settings → Pages**, choisissez `Deploy from a branch`, branche `main`, dossier `/ (root)`, puis enregistrez.
4. Après déploiement, les pages seront généralement accessibles à :
   - `https://VOTRE-PSEUDO.github.io/mottelo-legal/`
   - `https://VOTRE-PSEUDO.github.io/mottelo-legal/privacy-policy.html`
   - `https://VOTRE-PSEUDO.github.io/mottelo-legal/data-safety.html`
   - `https://VOTRE-PSEUDO.github.io/mottelo-legal/terms.html`
   - `https://VOTRE-PSEUDO.github.io/mottelo-legal/account-deletion.html`

## Hypothèses à vérifier

Le contenu part du contexte connu : authentification Supabase par e-mail/mot de passe, profil/pseudonyme et données de progression synchronisées. Les achats, publicités, outils d'analyse, journaux techniques, pièces jointes et transferts éventuels ne sont pas déclarés comme certains : confirmez ce que l'application utilise réellement et ajustez les pages ainsi que Play Console.
