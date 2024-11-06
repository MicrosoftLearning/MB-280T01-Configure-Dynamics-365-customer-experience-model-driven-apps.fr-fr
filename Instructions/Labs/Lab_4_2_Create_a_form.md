---
lab:
  title: "Labo\_4.2\_: créer des formulaires"
---

# Labo 4.2 : créer des formulaires

## Scénario
Bellows College est un établissement d’enseignement avec plusieurs campus et plusieurs cursus. De nombreux enseignants et administrateurs de Bellow College doivent assister à des événements et acheter des articles. Le suivi de ces dépenses a toujours été un défi en soi.
L’administration des campus aimerait moderniser son système de notes de frais en fournissant aux employés un moyen numérique de soumettre leurs dépenses.
Tout au long de ce cours, vous allez créer des applications et effectuer une automatisation pour permettre aux employés de Bellows College de gérer les dépenses.

## Étapes de labo de haut niveau
Après avoir terminé avec succès ce labo, vous aurez appris ce qui suit :
- personnaliser le formulaire de tableau pour qu’il réponde au mieux à vos besoins.

Nous travaillerons avec les composants suivants :
- Formulaires : C’est là que l’utilisateur crée ou met à jour de nouvelles lignes dans les tables.

## Prérequis
- Participation au Module 1 Labo 0 – Valider l’environnement de labo

## Exercice 1 : personnaliser les affichages et les formulaires
**Objectif** : Au cours de cet exercice, vous apprendrez à personnaliser les vues et les formulaires des tables personnalisées qui seront utilisées dans l’application pilotée par modèle.

### Tâche n°1 : Modifier le formulaire de notes de frais
1. Si ce n’est pas déjà fait, connectez-vous à `https://make.powerapps.com`.
2. Sélectionnez l’environnement dans lequel vous avez importé la solution Note de frais en haut à droite si elle n’est pas déjà sélectionnée.
3. Dans le volet de navigation de gauche, sélectionnez **Solutions.**
4. Ouvrez la solution Note de frais.
5. Recherchez et sélectionnez la table Notes de frais.
6. Sous la section Expériences des données, sélectionnez **Formulaires**, puis ouvrez le formulaire « Informations » avec le type de formulaire « Principal ». (Important : Veillez à sélectionner le formulaire de type Principal.)

**IMPORTANT :** par défaut, tous les formulaires portent le nom Informations. Assurez-vous donc de sélectionner le formulaire de type Principal et non un autre. Le formulaire comporte deux champs par défaut : « Nom » et « Propriétaire ».

### Tâche n° 2 : sélectionner des colonnes pour le formulaire
1. À droite de l’écran, dans le panneau Propriétés, sélectionnez le champ **Nom**, puis remplacez-le par `Report Information`.
2. Sélectionnez **Colonnes de la table** dans le volet de navigation gauche et ajoutez les champs suivants sous le champ Propriétaire en faisant glisser les colonnes dans le formulaire ou en cliquant simplement sur les noms de colonne :
    - Description
    - Objet de la note
    - Date d’échéance de la note
    - Total de la note
3. Glissez-déplacez la colonne **Raison du statut** dans l’en-tête du formulaire. L’en-tête est la zone supérieure droite du formulaire. Vous devrez peut-être réduire le panneau Propriétés sur le côté droit de l’écran pour voir le champ sur le formulaire.
4. Faites glisser la colonne **Dernière date d’approbation** et déposez-la à côté de Motif du statut dans l’en-tête du formulaire.
5. Sélectionnez le champ **Propriétaire**. Dans le panneau Propriétés, remplacez Étiquette par *`Requestor`*.
6. Dans le volet de navigation de gauche, sélectionnez **Composants**.
7. Sélectionnez la section de 1 colonne à ajouter sous la section active.
8. Dans l’écran Propriétés, remplacez l’étiquette par **`Expense Lines`**.
9. Avec la section Ligne de dépense toujours sélectionnée, recherchez et sélectionnez le composant **Subgrid**.
10. Cochez la case **Afficher les enregistrements connexes**.
11. Définissez la table sur **Lignes de dépenses (Note de frais).**
12. Définissez l’affichage par défaut sur **Lignes de dépenses actives.**
13. Cliquez sur **Terminé**.
14. Sélectionnez le bouton **Enregistrer et publier** en haut à droite et attendez la fin de l’opération d’enregistrement et de publication.
15. Sélectionnez le bouton de retour en haut à gauche de l’écran. Vous devriez normalement être revenu aux Formulaires de la table Note de frais.

### Tâche n° 3 : modifier le formulaire de ligne de dépense active
Dans cette tâche, nous allons modifier le formulaire utilisé pour ajouter des éléments de ligne de dépense.

1. Si ce n’est pas déjà fait, connectez-vous à `https://make.powerapps.com`
2. Sélectionnez l’environnement dans lequel vous avez importé la solution Note de frais en haut à droite si elle n’est pas déjà sélectionnée.
3. Dans le volet de navigation de gauche, sélectionnez Solutions
4. Ouvrez la solution Note de frais.
5. Recherchez et ouvrez la table Ligne de dépense.
6. Sous la section Expériences des données, sélectionnez Formulaires, puis ouvrez le formulaire Informations avec le type de formulaire Principal. (Important : Veillez à sélectionner le formulaire de type Principal.)

**IMPORTANT :** par défaut, tous les formulaires portent le nom Informations. Assurez-vous donc de sélectionner le formulaire de type Principal et non un autre. Le formulaire comporte deux champs par défaut : Titre de la dépense et Propriétaire.

1. À droite de l’écran, dans le panneau **Propriétés**, sélectionnez le champ **Nom d’affichage**, puis remplacez-le par `Item Details`.
2. Sélectionnez **Colonnes de la table** dans le volet de navigation gauche et ajoutez les champs suivants sous le champ Propriétaire en faisant glisser les colonnes dans le formulaire ou en cliquant simplement sur les noms de colonne :
    - Type de dépense
    - Description de l’élément
    - Montant de la dépense
    - Note de frais
3. Glissez-déplacez la colonne **Raison du statut** dans l’en-tête du formulaire. L’en-tête est la zone supérieure droite du formulaire. Vous devrez peut-être réduire le panneau Propriétés sur le côté droit de l’écran pour voir le champ sur le formulaire.
4. Cliquez sur le bouton **Enregistrer et publier**.
