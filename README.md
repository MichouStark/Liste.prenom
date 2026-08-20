# 👶 Le prénom de bébé

Petite application web (un seul fichier `index.html`, sans serveur ni base de données) pour confronter vos listes de prénoms et choisir ensemble.

## Utilisation

1. Ouvrez `index.html` dans un navigateur (en local, ou hébergé sur GitHub Pages / n'importe quel hébergeur statique).
2. Renseignez votre prénom.
3. Saisissez vos 10 prénoms filles et 10 prénoms garçons (un par ligne).
4. À l'étape **Partager**, copiez le lien généré et envoyez-le à votre partenaire (SMS, message...). Quand iel l'ouvre, l'app lui propose d'importer votre liste.
5. Une fois les deux listes présentes (dans le navigateur de chacun), l'étape **Comparaison** met en évidence les prénoms en commun. Un bouton **Exporter la liste complète** permet de copier/télécharger un récapitulatif texte de toutes les listes.
6. L'étape **Tri** permet à chacun de marquer n'importe quel prénom (commun ou non) comme à garder ❤️ ou à éliminer 🚫. Un prénom éliminé par l'un des deux disparaît de la sélection finale, même s'il n'est pas en commun ; un désaccord (l'un garde, l'autre élimine) est mis en évidence.
7. Chacun choisit son top 2 filles / top 2 garçons dans **Choix final** (parmi les prénoms non éliminés), puis repartage son code mis à jour.
8. L'étape **Récap** affiche les prénoms sur lesquels vous êtes tombés d'accord 🎉.

## Comment ça marche techniquement

- Toutes les données restent **dans le navigateur** (`localStorage`) et sont enregistrées automatiquement au fur et à mesure de la saisie (un petit badge "💾 Enregistré" confirme la sauvegarde) — rien n'est envoyé sur un serveur.
- Le partage se fait via un **lien contenant vos données encodées** (après le `#import=`), pas besoin de backend ni de compte.
- Vous pouvez héberger ce fichier tel quel sur GitHub Pages pour avoir un lien stable, ou simplement vous l'envoyer par e-mail/message et l'ouvrir localement.

## Déployer sur GitHub Pages (optionnel)

1. Poussez ce dépôt sur GitHub.
2. Dans les paramètres du dépôt → *Pages*, choisissez la branche et le dossier racine.
3. Votre app sera accessible à une URL du type `https://<utilisateur>.github.io/<repo>/`.
