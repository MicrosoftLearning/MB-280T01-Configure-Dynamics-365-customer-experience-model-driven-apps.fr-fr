---
lab:
  title: "Labo\_4.1\_: visualiser des données avec des vues"
---

# Labo 4.1 : visualiser des données avec des vues

## Scénario

Bellows College est un établissement d’enseignement avec plusieurs campus et plusieurs cursus. De nombreux enseignants et administrateurs de Bellow College doivent assister à des événements et acheter des articles. Le suivi de ces dépenses a toujours été un défi en soi.

L’administration des campus aimerait moderniser son système de notes de frais en fournissant aux employés un moyen numérique de soumettre leurs dépenses.

Tout au long de ce cours, vous allez créer des applications et effectuer une automatisation pour permettre aux employés de Bellows College de gérer les dépenses.

## Étapes de labo de haut niveau

Dans le cadre de la création de l’application basée sur un modèle, vous effectuerez les opérations suivantes :

créer différentes vues pour afficher les éléments des notes de frais.

Nous travaillerons avec les composants suivants :

Vues : Les vues permettent à l’utilisateur d’afficher les données existantes dans la table des formulaires.

## Prérequis

Participation au Module 1 Labo 0 - Valider l’environnement de labo

## Exercice 1 : gérer les vues

**Objectif :**  dans cet exercice, vous allez créer une nouvelle vue qui peut être utilisée ultérieurement dans les applications pilotées par modèles.

### Tâche n° 1 : modifier les différentes vues de Lignes de dépenses

1. Si ce n’est pas déjà fait, connectez-vous à  `https://make.powerapps.com`.
2. Sélectionnez l’environnement dans lequel vous avez importé la solution Note de frais en haut à droite si elle n’est pas déjà sélectionnée.
3. Dans le volet de navigation de gauche, sélectionnez **Solutions.**
4. Ouvrez la solution Note de frais.
5. Recherchez et ouvrez la table Ligne de dépense.
6. Sous Expériences de données, sélectionnez **Vues.**
7. Ouvrez la vue **Lignes de dépenses actives**.
8. Cliquez sur **Sélectionner Afficher la colonne.** Sélectionnez **Date de la dépense, Description de l'élément, Type de dépense,** et **Montant de la dépense.**
9. Recherchez et sélectionnez la colonne **Créée le**. Dans le menu qui s’affiche, sélectionnez **Supprimer**.
10. Votre vue doit contenir les colonnes Titre de la dépense, Date de la dépense, Description de l’élément, Type de dépense et Montant de la dépense.
11. Sélectionnez le bouton **Enregistrer et publier**.
12. En sélectionnant le bouton de retour, vous revenez à la liste des vues.

Ensuite, ce processus est répété pour actualiser la vue associée la ligne de dépense. Il s’agit de la vue qui s’affiche lorsque vous examinez les lignes de dépenses à partir d’une table parente telle que Note de frais.

### Tâche n° 2 : mettre à jour la vue associée à la ligne de dépense 

1. Recherchez et ouvrez la vue associée à la ligne de dépense.
2. Cliquez sur **Sélectionner Afficher la colonne.** Sélectionnez **Date de la dépense, Description de l'élément, Type de dépense,** et **Montant de la dépense.**
3. Recherchez et sélectionnez la colonne **Créée le**. Dans le menu qui s’affiche, sélectionnez **Supprimer**.
4. Votre vue doit contenir les colonnes Titre de la dépense, Date de la dépense, Description de l’élément, Type de dépense et Montant de la dépense.
5. Sélectionnez le bouton **Enregistrer et publier**.
6. En sélectionnant le bouton de retour, vous revenez à la liste des vues.

Enfin, ce processus est répété encore une fois pour actualiser la vue Recherche rapide des lignes de dépenses actives. Il s’agit de la vue affichée chaque fois qu’un utilisateur recourt au champ de recherche pour trouver une ligne de dépense spécifique.

### Tâche n° 3 : mettre à jour la vue Recherche rapide

1. Recherchez et ouvrez la vue Recherche rapide des lignes de dépenses actives.
2. Cliquez sur **Sélectionner Afficher la colonne.** Sélectionnez **Date de la dépense, Description de l'élément, Type de dépense,** et **Montant de la dépense.**
3. Recherchez et sélectionnez la colonne **Créée le**. Dans le menu qui s’affiche, sélectionnez **Supprimer**.
4. Votre vue doit contenir les colonnes Titre de la dépense, Date de la dépense, Description de l’élément, Type de dépense et Montant de la dépense.
5. Sur le côté droit de l’écran, dans la section Rechercher par, sélectionnez **Modifier les colonnes de la table de recherche.**
6. Ajoutez les colonnes suivantes :
    - Date de la dépense
    - Type de dépense
7. Sélectionnez le bouton **Appliquer**.
8. Sélectionnez le bouton **Enregistrer et publier**.
9. En sélectionnant le bouton de retour, vous revenez à la liste des vues.

### Tâche n° 4 : modifier les différentes vues de Notes de frais

1. Si ce n’est pas déjà fait, connectez-vous à  `https://make.powerapps.com`.
2. Sélectionnez l’environnement dans lequel vous avez importé la solution Note de frais en haut à droite si elle n’est pas déjà sélectionnée.
3. Dans le volet de navigation de gauche, sélectionnez **Solutions.**
4. Ouvrez la solution Note de frais.
5. Recherchez et sélectionnez la table Notes de frais.
6. Sous Expériences de données, sélectionnez **Vues.**
7. Ouvrez la vue **Notes de frais actives**.
8. Cliquez sur **Sélectionner Afficher la colonne.** Sélectionnez **Objectif du rapport, Date d’échéance du rapport, Total du rapport** et **Dernière date d’approbation**.
9. Recherchez et sélectionnez la colonne **Créée le**. Dans le menu qui s’affiche, sélectionnez **Supprimer**.
10. Votre vue doit comporter les colonnes Objet du rapport, Date d’échéance du rapport, Total du rapport et Dernière date d’approbation.
11. Sélectionnez le bouton **Enregistrer et publier**.
12. En sélectionnant le bouton de retour, vous revenez à la liste des vues.

Ensuite, ce processus est répété pour actualiser la vue Note de frais inactives.

### Tâche n° 5 : mettre à jour la vue Notes de frais inactives

1. Recherchez et ouvrez la vue Notes de frais inactives.
2. Cliquez sur **Sélectionner Afficher la colonne.** Sélectionnez **Objectif du rapport, Date d’échéance du rapport, Total du rapport** et **Dernière date d’approbation**.
3. Recherchez et sélectionnez la colonne **Créée le**. Dans le menu qui s’affiche, sélectionnez **Supprimer**.
4. Votre vue doit comporter les colonnes Objet du rapport, Date d’échéance du rapport, Total du rapport et Dernière date d’approbation.
5. Sélectionnez le bouton **Enregistrer et publier**.
6. En sélectionnant le bouton de retour, vous revenez à la liste des vues.

### Tâche n° 6 : mettre à jour la vue Recherche rapide des notes de frais actives 

Enfin, ce processus est répété encore une fois pour actualiser la vue Recherche rapide des notes de frais actives. Il s’agit de la vue affichée chaque fois qu’un utilisateur recourt au champ de recherche pour trouver une note de frais spécifique.

1. Recherchez et ouvrez la vue Recherche rapide des notes de frais actives.
2. Cliquez sur **Sélectionner Afficher la colonne.** Sélectionnez **Objectif du rapport, Date d’échéance du rapport, Total du rapport** et **Dernière date d’approbation**.
3. Recherchez et sélectionnez la colonne **Créée le**. Dans le menu qui s’affiche, sélectionnez **Supprimer**.
4. Votre vue doit comporter les colonnes Objet du rapport, Date d’échéance du rapport, Total du rapport et Dernière date d’approbation.
5. Sur le côté droit de l’écran, dans la section Rechercher par, sélectionnez **Modifier les colonnes de la table de recherche.**
6. Ajoutez la colonne Objectif du rapport.
7. Sélectionnez le bouton **Appliquer**.
8. Sélectionnez le bouton **Enregistrer et publier**.
9. En sélectionnant le bouton de retour, vous revenez à la liste des vues.

### Tâche n° 7: créer une vue appelée Notes de frais dues aujourd’hui

1. Si ce n’est pas déjà fait, connectez-vous à  `https://make.powerapps.com`.
2. Sélectionnez l’environnement dans lequel vous avez importé la solution Note de frais en haut à droite si elle n’est pas déjà sélectionnée.
3. Dans le volet de navigation de gauche, sélectionnez **Solutions.**
4. Ouvrez la solution Note de frais.
5. Recherchez et sélectionnez la table Notes de frais.
6. Sous Expériences de données, sélectionnez **Vues.**
7. Ouvrez la vue Notes de frais actives.
8. Sélectionnez le bouton **Enregistrer sous**.
9. Modifiez le nom en *`Expense Reports Due Today`*.
10. Sélectionnez le bouton **Enregistrer**.
11. Dans la section Filtrer par, sélectionnez **Modifier les filtres.**
12. Cliquez sur le bouton **Ajouter**. Dans le menu qui s’affiche, sélectionnez **Ajouter une ligne**.
13. Sélectionnez la flèche déroulante dans la première ligne vide. Dans le menu qui s’affiche, sélectionnez la colonne **Notes de frais dues aujourd’hui**.
14. Modifiez le champ Égal en **Aujourd’hui.**
15. Cliquez sur le bouton **OK**.
16. Cliquez sur le bouton **Enregistrer et publier**.
