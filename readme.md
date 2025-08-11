# 🧰 Aide-mémoire Git

## Initialisation & ajout de fichiers

- `git init`  
  Initialise un nouveau dépôt Git dans le dossier courant.

- `git add <nom_fichier>`  
  Ajoute un fichier spécifique à la zone de staging (préparation pour commit).

- `git add .`  
  Ajoute tous les fichiers modifiés/non suivis dans la zone de staging.

---

## Commit & historique

- `git commit -m "message de commit"`  
  Enregistre les fichiers en staging dans l'historique local avec un message clair.

- `git status`  
  Affiche l’état des fichiers (modifiés, en staging, non suivis).

- `git log`  
  Affiche la liste complète des commits.

- `git log --oneline`  
  Affiche un résumé des commits, un par ligne, avec leur identifiant court.

---

## Gestion des branches

- `git branch`  
  Liste les branches locales, indique la branche courante.

- `git branch <nom_branche>`  
  Crée une nouvelle branche locale.

- `git checkout <nom_branche>`  
  Change la branche courante.

- `git switch <nom_branche>`  
  Alternative moderne pour changer la branche courante.

- `git branch -d <nom_branche>`  
  Supprime une branche locale (ne fonctionne que si elle est mergée).

- `git branch -D <nom_branche>`  
  Supprime une branche locale **forcément**, même si elle n’est pas mergée.

- `git push origin --delete <nom_branche>`  
  Supprime une branche distante sur GitHub.

- `git push --set-upstream origin <nom_branche>`  
  Pousse la branche locale sur GitHub et établit la relation de suivi.

---

## Configuration des dépôts distants & push

- `git remote add origin <url>`  
  Configure l’URL du dépôt distant (à faire une seule fois).

- `git remote -v`  
  Liste les dépôts distants configurés.

- `git push`  
  Envoie les commits locaux vers le dépôt distant (branchée avec upstream).

- `git push origin <nom_branche>`  
  Envoie une branche spécifique vers le dépôt distant.

- `git pull`  
  Récupère les modifications distantes et les fusionne dans la branche locale.

---

## Annuler et revenir en arrière

- `git reset HEAD <fichier>`  
  Retire un fichier de la zone de staging (préparation).

- `git checkout -- <fichier>`  
  Annule les modifications locales non commités sur un fichier.

- `git revert <commit>`  
  Crée un nouveau commit annulant les modifications d’un commit passé.

- `git reset --hard <commit>`  
  Replace la branche à un commit précédent et supprime les changements locaux (dangereux).

---

## Autres commandes utiles

- `git stash`  
  Sauvegarde temporairement les modifications non commités.

- `git stash pop`  
  Récupère les modifications sauvegardées et les supprime du stash.

- `git fetch`  
  Récupère les données du dépôt distant sans fusionner.

---

## Supprimer une branche

```bash
# Supprimer une branche distante (GitHub)
git push origin --delete <nom_branche>

# Supprimer une branche locale
git branch -d <nom_branche>       # Supprime si branch mergée
git branch -D <nom_branche>       # Supprime forcé même si non mergée
```


## Images

<img src="image/images.jpeg" alt="image de github" width="200"/>

## Lien cliquable 
<a href="https://markdownlivepreview.com/">
 Markdownlivepreview 
</a>

## Blockquotes

> Markdown is a lightweight markup language with plain-text-formatting syntax, created in 2004 by John Gruber with Aaron Swartz.
>
>> Markdown is often used to format readme files, for writing messages in online discussion forums, and to create rich text using a plain text editor.

## Tables

| Left columns  | Right columns |
| ------------- |:-------------:|
| left foo      | right foo     |
| left bar      | right bar     |
| left baz      | right baz     |

## Blocks of code

```
let message = 'Hello world';
alert(message);
```

## Inline code 
Pour initialiser un dépôt git, tapez la commande `git init`.

