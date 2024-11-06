---
lab:
  title: "Labo\_2.1\_: créer des champs calculés et cumulatifs"
---

# Labo 2.1 : créer des champs calculés et cumulatifs 

## Scénario
Bellows College est un établissement d’enseignement avec plusieurs campus et plusieurs cursus. De nombreux enseignants et administrateurs de Bellow College doivent assister à des événements et acheter des articles. Le suivi de ces dépenses a toujours été un défi en soi.
L’administration des campus aimerait moderniser son système de notes de frais en fournissant aux employés un moyen numérique de soumettre leurs dépenses.
Dans l’idéal, elle veut que leurs utilisateurs remplissent une note de frais après chaque événement ou achat. Pour chaque note de frais, elle veut qu’ils puissent ajouter des éléments de ligne de dépenses individuels. Elle a déjà commencé à travailler sur cette solution. La table Note de frais a été créée. Vous avez été invité à reprendre le projet et à le terminer.

## Étapes de labo de haut niveau
À l’issue de ce labo, vous pourrez :
- Ajouter de nouveaux champs à une table existante
- Création d’un champ cumulatif
- Créer un champ calculé

## Prérequis
- Achèvement du module 1 du Labo 0 - Valider l’environnement de labo et Labo 1.1, où vous avez importé la solution Note de frais

## Éléments à considérer avant de commencer
- Conventions d’affectation de noms : tapez les noms sans aucune erreur.

## Exercice 1 : créer des champs calculés et cumulatifs
**Objectif :** dans cet exercice, créez un champ calculé et un champ cumulatif dans la table des notes de frais.

### Tâche n°1 : ajouter un champ cumulatif à la table Note de frais
1. Si nécessaire, accédez au portail Power Apps Maker.
2. Assurez-vous que vous travaillez dans l’environnement dans lequel vous avez importé la solution Note de frais pendant le dernier exercice.
3. Dans le volet de navigation de gauche, sélectionnez **Solutions.**
4. Recherchez et sélectionnez la solution de notes de frais.
5. Recherchez et sélectionnez la table Notes de frais.
6. En dessous de Schéma, sélectionnez **Colonnes**.
7. Sélectionnez **+ Nouvelle colonne**.
8. Entrez *`Report Total`* comme Nom d’affichage.
9. Sélectionnez **Devise** comme type de données.
10. Dans Obligatoire, sélectionnez **Facultatif.**
11. Dans le champ Comportement, sélectionnez **Cumul.**
12. Sélectionnez le bouton **Enregistrer**. (Vous devez enregistrer la colonne avant de pouvoir la configurer.)
13. Une fois la colonne enregistrée, une fenêtre contextuelle apparaît. (Si vous recevez un message contextuel, vous devrez peut-être autoriser les fenêtres contextuelles.)
14. Sous ENTITÉ ASSOCIÉE, sélectionnez **+ Ajouter une entité associée.**
15. Sélectionnez **(Lignes de dépenses) Note de frais.**
16. Sélectionnez le bouton en forme de coche pour accepter la modification.
17. Sous AGRÉGATION, sélectionnez **+ Ajouter une agrégation.**
18. Définissez la fonction d’agrégation sur **Somme.**
19. Définissez le champ de l'entité apparentée agrégée sur **(Ligne de dépenses) Montant des dépenses.**
20. Sélectionnez la coche verte, puis le bouton **Enregistrer et fermer**.

### Tâche n°2 : ajouter un champ Formule calculée de Power FX à la table Notes de frais
1. Si nécessaire, accédez au portail Power Apps Maker.
2. Assurez-vous que vous travaillez dans l’environnement dans lequel vous avez importé la solution Note de frais pendant le dernier exercice.
3. Dans le volet de navigation de gauche, sélectionnez **Solutions.**
4. Recherchez et sélectionnez la solution de notes de frais.
5. Recherchez et sélectionnez la table Notes de frais.
6. En dessous de Schéma, sélectionnez **Colonnes**.
7. Sélectionnez **+ Nouvelle colonne**.
8. Entrez *`Last Date for approval`* comme Nom d’affichage.
9. Sélectionnez **Formule** pour le type de données.
10. Entrez la formule suivante : `DateAdd('Report Due Date',2)`.
11. Définissez le champ Format sur **Date uniquement.**
12. Sélectionnez le bouton **Enregistrer**. (Vous devez enregistrer la colonne avant de pouvoir la configurer.)
