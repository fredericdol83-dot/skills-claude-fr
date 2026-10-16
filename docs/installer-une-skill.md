# Installer une skill

Une skill est un dossier qui contient au minimum un fichier `SKILL.md`. Son en-tête donne un nom et une description. Claude lit la description pour savoir quand utiliser la skill, puis suit les instructions du fichier.

## 1. Récupérer le dossier

Sur la page d'accueil du dépôt, cliquez sur le bouton vert « Code », puis « Download ZIP ». Décompressez l'archive. Chaque skill est un sous-dossier de `skills/`.

## 2a. Dans Claude (site web ou application)

1. Compressez le dossier de la skill seul en .zip (par exemple `nouvelle-idee.zip`, qui contient `SKILL.md` et éventuellement `references/`).
2. Dans Claude, ouvrez les paramètres et cherchez la rubrique des skills (dans les capacités, selon la version).
3. Importez le .zip et vérifiez que la skill est activée.

Les libellés exacts de l'interface changent de temps en temps. Si vous ne trouvez pas la rubrique, demandez directement à Claude où importer une skill.

## 2b. Dans Claude Code

Copiez le dossier de la skill :
- dans `~/.claude/skills/` pour qu'elle serve dans tous vos projets ;
- ou dans `.claude/skills/` à la racine d'un projet pour la limiter à celui-ci.

Relancez Claude Code. La skill apparaît dans la liste et se déclenche quand votre demande correspond à sa description. Vous pouvez aussi l'appeler par son nom.

## 3. L'adapter à vous

Ouvrez `SKILL.md` dans n'importe quel éditeur de texte. Modifiez le portrait de l'utilisateur, vos outils ou vos règles. La description en haut du fichier est la partie la plus importante : si la skill ne se déclenche pas quand vous le voulez, c'est elle qu'il faut reformuler.
