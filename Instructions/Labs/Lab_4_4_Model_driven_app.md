---
lab:
  title: "Labo\_4.4\_: créer une application pilotée par modèle"
---

# Labo 4.4 : créer une application pilotée par modèle

## Scénario
Bellows College est un établissement d’enseignement avec plusieurs campus et plusieurs cursus.

De nombreux enseignants et administrateurs de Bellow College doivent assister à des événements et acheter des articles. Le suivi de ces dépenses a toujours été un défi en soi.
L’administration des campus aimerait moderniser son système de notes de frais en fournissant aux employés un moyen numérique de soumettre leurs dépenses.

Tout au long de ce cours, vous allez créer des applications et effectuer une automatisation pour permettre aux employés de Bellows College de gérer les dépenses.

## Étapes de labo de haut niveau
Dans le cadre de la configuration de l’application pilotée par modèle, vous effectuerez les opérations suivantes :
- configurer votre nouvelle application pilotée par modèle nommée Gestion des dépenses des employés.

Nous travaillerons avec les composants suivants :
- Vues : Les vues permettent à l’utilisateur d’afficher les données existantes dans la table des formulaires.
- Formulaires : C’est là que l’utilisateur crée ou met à jour de nouvelles lignes dans les tables.
Les deux seront intégrés à l’application basée sur un modèle, pour une meilleure expérience utilisateur.

## Prérequis
- Participation au Module 1 Labo 0 – Valider l’environnement de labo

## Exercice 1 : créer une application pilotée par modèle
**Objectif :** dans cet exercice, vous utiliserez l’application pilotée par modèle que vous avez configurée dans le Labo 4.3. Vous personnaliserez ensuite le plan du site et testerez l’application.
Pour rester simples et gagner du temps, nous n’aborderons pas toutes les colonnes Note de frais dans ce labo.

## Tâche 1 : configurer le plan du site
1. Si ce n’est pas déjà fait, connectez-vous à `https://make.powerapps.com`.
2. Sélectionnez l’environnement dans lequel vous avez importé la solution Note de frais en haut à droite si elle n’est pas déjà sélectionnée.
3. Dans le volet de navigation de gauche, sélectionnez **Solutions.**
4. Ouvrez la solution Note de frais.
5. Recherchez l’application *`Employee Expense Management`* que vous avez créée dans le dernier exercice.
6. Sélectionnez **Modifier** pour ouvrir le concepteur d’application moderne.
7. Dans la barre de commandes, sélectionnez **+Ajouter une page**.
8. L‘écran **Ajouter une page** apparaît.
9. Choisissez **la table Dataverse.**
10. Sélectionnez les tables suivantes :
    - Note de frais
    - Ligne de dépense
11. Assurez-vous que l’option Afficher dans la navigation est sélectionnée.
12. Une fois que vous avez sélectionné les 2 tables, sélectionnez **Ajouter.**
13. Sous Navigation, sélectionnez le formulaire **Notes de frais**.
14. Accédez à la section Dans cette application sur le côté droit de l’écran.
15. Sélectionnez **Afficher plus**.
16. Sélectionnez les **points de suspension** à côté de l’aperçu.
17. Dans le menu qui s’affiche, sélectionnez **Supprimer**.
18. Sélectionnez les **points de suspension** à côté du formulaire de carte d’informations.
19. Dans le menu qui s’affiche, sélectionnez **Supprimer**.
20. Sous Navigation, sélectionnez le formulaire **Lignes de dépenses**.
21. Accédez à la section Dans cette application sur le côté droit de l’écran.
22. Sélectionnez **Afficher plus**.
23. Sélectionnez les **points de suspension** à côté de l’aperçu.
24. Dans le menu qui s’affiche, sélectionnez **Supprimer**.
25. Sélectionnez les **points de suspension** à côté du formulaire de carte d’informations.
26. Dans le menu qui s’affiche, sélectionnez **Supprimer**.
27. Sélectionnez **Enregistrer** et attendez la fin de l’enregistrement.
28. Une fois la sauvegarde terminée, sélectionnez le bouton **Publier** pour publier vos modifications. Attendez la fin de la publication.

### Tâche 2 : Tester l’application
**Démarrer l’application**
1. Sélectionnez le bouton Lecture pour charger l’application pilotée par modèle dans un nouvel onglet.

**Créer une note de frais**
1. Sélectionnez **Notes de frais** dans la navigation de gauche (également appelée « plan du site »).
2. Cliquez sur **+ Nouveau**.
3. Renseignez les champs comme suit :
    - Nom du rapport : **`New Test Report`**
    - Objectif du rapport : sélectionnez **`Conference`**
    - Date d’échéance du rapport : sélectionnez **`Today's date`**
4. Cliquez sur **Enregistrer et fermer**. Cette opération crée un rapport de test que vous devriez voir dans la vue Notes de frais actives.
5. Passez à la vue **Notes de frais dues aujourd’hui** en utilisant la liste déroulante à côté de Notes de frais actives.
6. Vous pouvez ajouter quelques autres enregistrements de test.

Votre application pilotée par modèle en cours d’exécution doit ressembler à ceci :

![une capture d’écran d’une application pilotée par modèle](./Media/Model_driven_apps.png)

Félicitations ! Vous avez créé et configuré votre première application pilotée par modèle.
