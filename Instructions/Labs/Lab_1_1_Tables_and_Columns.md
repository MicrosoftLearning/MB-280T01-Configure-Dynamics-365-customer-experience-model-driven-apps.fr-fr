---
lab:
  title: "Labo\_1.1\_: créer et gérer des tables et des colonnes"
---

# Labo 1.1 : créer et gérer des tables et des colonnes

## Scénario
Bellows College est un établissement d’enseignement avec plusieurs campus et plusieurs cursus. De nombreux enseignants et administrateurs de Bellow College doivent assister à des événements et acheter des articles. Le suivi de ces dépenses a toujours été un défi en soi.
L’administration des campus aimerait moderniser son système de notes de frais en fournissant aux employés un moyen numérique de soumettre leurs dépenses.
Dans l’idéal, elle veut que leurs utilisateurs remplissent une note de frais après chaque événement ou achat. Pour chaque note de frais, elle veut qu’ils puissent ajouter des éléments de ligne de dépenses individuels. Elle a déjà commencé à travailler sur cette solution. La table Note de frais a été créée. Vous avez été invité à reprendre le projet et à le terminer.

## Étapes de labo de haut niveau
À l’issue de ce labo, vous pourrez :
- Importer une solution dans votre environnement qui inclut la table Notes de frais.
- Créer une table d’éléments de ligne de dépense.
- Ajouter les colonnes nécessaires à la table d’éléments de ligne de dépense.
- Ajoutez des exemples de données.

## Prérequis
- Conclusion du Module 1 Lab 0 – Valider l'environnement de laboratoire 

## Éléments à considérer avant de commencer
- Conventions d’affectation de noms : tapez les noms sans aucune erreur.

## Excercice 1: importer la solution de notes de frais dans votre environnement
**Objectif :** dans cet exercice, vous allez importer la solution de notes de frais qui inclut la table Notes de frais.

### Tâche 1 : importer la solution
La table Notes de frais contiendra des informations sur les notes de frais que la personne envoie.
1. Si vous n’êtes pas encore connecté, connectez-vous à `make.powerapps.com` l’aide de vos informations d’identification d’environnement.
2. Dans le menu Environnement en haut à droite, vérifiez que vous êtes dans l’environnement dans lequel vous souhaitez importer la solution.
3. Dans le volet de navigation de gauche, sélectionnez **Solutions.**
4. Dans la barre de commandes en haut, sélectionnez **Importer une solution**.
5. Cliquez sur le bouton **Parcourir**.
6. Recherchez et sélectionnez le fichier de solution `ExpenseReport_1_0_0_1` situé dans vos documents de cours.
7. Sélectionnez le bouton **Importer**.

*Remarque : l’importation de la solution dans votre environnement peut prendre plusieurs minutes.*

## Exercice 2 : créer des tables et des colonnes
**Objectif :** dans cet exercice, vous allez importer la solution de notes de frais qui inclut la table Notes de frais.

### Tâche 1 : créer une table de lignes de dépenses
1. Si nécessaire, accédez au portail Power Apps Maker.
2. Assurez-vous que vous travaillez dans l’environnement dans lequel vous avez importé la solution `ExpenseReport_1_0_0_1` pendant le dernier exercice.
3. Dans le volet de navigation de gauche, sélectionnez **Solutions.**
4. Recherchez et sélectionnez la solution de notes de frais.
5. Sélectionnez le bouton **Nouveau**.
6. Dans le menu qui s’affiche, accédez à **Table.** Ensuite, sélectionnez **Table (propriétés avancées).**
7. Configurez votre nouvelle table comme suit :
   - Nom d’affichage : `Expense Line`
   - Nom pluriel : `Expense Lines`
   - Activer les pièces jointes (y compris les notes et les fichiers) : sélectionné
8. Cliquez sur l’onglet Colonne principale et modifiez Nom d’affichage par Titre de dépense.
9. Sélectionnez le bouton Enregistrer.

*Remarque : la création de la table peut prendre une ou deux minutes.*

### Tâche 2 : ajouter les colonnes nécessaires à la table de lignes de dépenses
1. Une fois la table de lignes de dépenses ouverte, sélectionnez Colonnes sous le groupe Schéma.
2. Sélectionnez **+ Nouvelle colonne**.
3. Saisissez **`Expense Type`** comme Nom d’affichage.
4. Sélectionnez **Choix > Choix** pour Type de données.
5. Dans Obligatoire, sélectionnez **Facultatif.**
6. Définissez Synchroniser avec le choix global sur **Oui (recommandé)**.
7. Dans le champ Synchroniser ce choix avec, cliquez sur **+ Nouveau choix.**
8. Dans le champ Nom d’affichage, saisissez *`Expense Type`*.
9. Dans le champ Étiquette du premier choix, saisissez *`Meals`*.
10. Sélectionnez **+ Nouveau choix**.
11. Dans le champ Étiquette, saisissez *`Lodging`*.
12. Répétez les étapes 10 et 11 pour ajouter les options suivantes :
    - `Travel`
    - `Entertainment`
    - `Supplies / Equipment`
    - `Other`
13. Sélectionnez le bouton **Enregistrer**.
14. Dans le champ Synchroniser ce choix avec, sélectionnez le choix **Type de dépense** que vous venez de créer.
15. Définissez le champ Choix par défaut sur **Aucun.**
16. Cliquez sur **Enregistrer**.

### Tâche 3 : créer une colonne Montant de la dépense
1. Sélectionnez + Nouvelle colonne.
2. Saisissez `Expense Amount` comme Nom d’affichage.
3. Sélectionnez Devise comme type de données.
4. Cliquez sur Enregistrer.

### Tâche 4 : créer une colonne Description de l’élément
1. Sélectionnez **+ Nouvelle colonne**.
2. Saisissez *`Item Description`* comme Nom d’affichage.
3. Sélectionnez **Plusieurs lignes de texte > Texte brut** pour Type de données.
4. Cliquez sur **Enregistrer**.

### Tâche 5 : créer une colonne Date de la dépense
1. Sélectionnez **+ Nouvelle colonne**.
2. Saisissez *`Expense Date`* comme Nom d’affichage.
3. Sélectionnez **Date uniquement** dans le groupe Date et Heure dans le champ Type de données.
4. Développer **Options avancées**.
5. Définissez le champ Ajustement du fuseau horaire sur **Heure locale de l’utilisateur.**
6. Cliquez sur **Enregistrer**.

### Tâche 6 : créer une colonne de note de frais
1. Sélectionnez **+ Nouvelle colonne**.
2. Saisissez *`Expense Report`* comme Nom d’affichage.
3. Sélectionnez **Recherche** depuis le groupe Recherche dans le champ Type de données.
4. Dans le champ Table associée, sélectionnez **Note de frais.**
5. Cliquez sur **Enregistrer**.

## Exercice 3 : modifier la table
**Objectif :** dans cet exercice, vous allez modifier manuellement une table.

### Tâche n°1 : Modifier les colonnes affichées
1. Si nécessaire, accédez au portail Power Apps Maker.
2. Assurez-vous que vous travaillez dans l’environnement dans lequel vous avez importé la solution **ExpenseReport_1_0_0_1** pendant le dernier exercice.
3. Dans le volet de navigation de gauche, sélectionnez **Solutions.**
4. Recherchez et sélectionnez la solution de **notes de frais**.
5. Dans le volet de navigation de gauche, sélectionnez **Tables**.
6. Ouvrez la table de lignes de dépenses que vous avez créée dans l’exercice précédent.
7. En regard de la colonne Séquence d’importation, sélectionnez **+[X] plus**. (Le nombre indiqué ici dépend de la taille de votre navigateur.)
8. Dans le menu qui s’affiche, sélectionnez les colonnes suivantes :
   - Montant de la dépense (base)
   - Date de la dépense (si elle n’est pas déjà sélectionnée)
   - Note de frais
   - Type de dépense
   - Montant de la dépense
   - Description de l’élément
9. Cliquez sur le bouton **Enregistrer**.
10. Recherchez la colonne **Créée par** et sélectionnez-la.
11. Dans le menu qui s’affiche, sélectionnez **Masquer.**
12. Répétez les étapes 10 et 11 pour supprimer les colonnes suivantes :
    - Créée par
    - Ligne de dépense
    - Séquence d’importation
