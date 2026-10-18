# CV Express

Page web de commande de CV professionnels pour étudiants et jeunes diplômés en RDC.
Le client choisit une offre, paie par Orange Money, puis envoie sa confirmation sur WhatsApp. Le CV est livré en PDF.

## Ce qu'il y a dans le projet

- `index.html` : toute la page (texte, style et petit programme JavaScript dans un seul fichier, sans installation).
- `README.md` : ce guide.

## Comment la page fonctionne

1. **Offres et tarifs** : 3 $, 5 $ ou 8 $. Le montant s'affiche automatiquement dans l'étape de paiement.
2. **Message WhatsApp automatique** : le formulaire construit un message prêt à envoyer (prénom, offre, poste visé, montant payé, référence de transaction) et l'ouvre dans WhatsApp grâce à un lien `wa.me`.
3. **Paiement Orange Money** : la page affiche le montant et ton numéro, avec un bouton pour le copier. La page ne reçoit pas l'argent et ne peut pas vérifier un paiement : l'argent arrive directement sur ton compte Orange Money.
4. **Livraison** : tu envoies le CV en PDF par WhatsApp, une fois le paiement vérifié.

## Vérifier un paiement (important)

- Regarde toujours **le SMS de confirmation que tu reçois toi-même** d'Orange Money et le solde de ton compte. Ne te fie jamais à la capture d'écran du client seule : une capture peut être falsifiée.
- Compare le montant et la référence de transaction avec ce que le client t'a envoyé.
- Ne livre le CV qu'après avoir vu l'argent arriver chez toi.

## Modifier la page

Ouvre `index.html` et cherche le bloc `À MODIFIER si besoin`, vers la fin du fichier :

- `WHATSAPP` : ton numéro WhatsApp au format international, sans `+` ni espaces.
- `NUMERO_OM` : le numéro Orange Money affiché aux clients.
- `NOM_COMPTE` : le nom du compte Orange Money, pour que le client vérifie avant d'envoyer l'argent.

Les prix se changent à deux endroits : la liste « Tarifs » et les options du menu « Offre ».

## Mettre le site en ligne avec GitHub Pages (depuis un téléphone)

1. Dans le navigateur du téléphone, va sur github.com et crée un compte gratuit.
2. Active « Version pour ordinateur » dans le menu du navigateur pour voir tous les boutons.
3. Clique sur **New repository**. Nom : `cv-express`. Choisis **Public**. Valide avec **Create repository**.
4. Clique sur **creating a new file**. Nomme-le `index.html`, colle tout le code, puis clique sur **Commit changes**.
5. Ajoute aussi `README.md` de la même façon (optionnel).
6. Va dans **Settings**, puis **Pages**. Dans « Source », choisis **Deploy from a branch**, branche **main**, dossier **/ (root)**, puis **Save**.
7. Attends 1 à 2 minutes. Ton lien sera : `https://TON-PSEUDO.github.io/cv-express/`

Tu peux ensuite partager ce lien en statut WhatsApp, dans des groupes d'étudiants et sur Facebook.

## Idées pour la suite

- Ajouter de vrais exemples de CV (avec l'accord des clients) et leurs avis.
- Proposer des offres : refaire un CV existant, traduction français-anglais, lettre seule.
- Garder un cahier des commandes (nom, offre, montant, date, statut) pour suivre tes gains.
