---
lab:
  title: "Labo\_4.3\_: créer un tableau de bord"
---

# Labo 4.3 : créer un tableau de bord 

## Scénario
Bellows College est un établissement d’enseignement avec plusieurs campus et plusieurs cursus. De nombreux enseignants et administrateurs de Bellow College doivent assister à des événements et acheter des articles. Le suivi de ces dépenses a toujours été un défi en soi.
L’administration des campus aimerait moderniser son système de notes de frais en fournissant aux employés un moyen numérique de soumettre leurs dépenses.
Tout au long de ce cours, vous allez créer des applications et effectuer une automatisation pour permettre aux employés de Bellows College de gérer les dépenses.

## Étapes de labo de haut niveau
À l’issue de ce labo, vous pourrez :
- Créer une application pilotée par modèle
- Créer un tableau de bord personnel qui affiche les informations de note de frais
- Ajouter vos vues et tableaux de bord à votre application pilotée par modèle

## Prérequis
- Participation au Module 1 Labo 0 – Valider l’environnement de labo

## Exercice 1 : créer un tableau de bord personnel

### Tâche 1 : créer votre application pilotée par modèle
1. Si ce n’est pas déjà fait, connectez-vous à `https://make.powerapps.com`.
2. Sélectionnez l’environnement dans lequel vous avez importé la solution Note de frais en haut à droite si elle n’est pas déjà sélectionnée.
3. Dans le volet de navigation de gauche, sélectionnez **Solutions.**
4. Ouvrez la solution Note de frais.
5. Dans la barre de commandes, sélectionnez le bouton **+ Nouveau**.
6. Dans le menu qui s’affiche, accédez à **Application > Application pilotée par modèle.**
7. Entrez *`Employee Expense Management`* comme Nom, puis sélectionnez **Créer.**

### Tâche n° 2 : créer une nouvelle vue appelée Mes notes de frais actives
1. Si ce n’est pas déjà fait, connectez-vous à `https://make.powerapps.com`.
2. Sélectionnez l’environnement dans lequel vous avez importé la solution Note de frais en haut à droite si elle n’est pas déjà sélectionnée.
3. Dans le volet de navigation de gauche, sélectionnez **Solutions.**
4. Ouvrez la solution Note de frais.
5. Recherchez et sélectionnez la table Notes de frais.
6. Sous Expériences de données, sélectionnez **Vues.**
7. Ouvrez la vue **Notes de frais actives**.
8. Sélectionnez le bouton **Enregistrer sous**.
9. Modifiez le nom en *`My Active Expense Reports`*.
10. Sélectionnez le bouton **Enregistrer**.
11. Dans la section Filtrer par, sélectionnez **Modifier les filtres.**
12. Cliquez sur le bouton **Ajouter**. Dans le menu qui s’affiche, sélectionnez **Ajouter une ligne**.
13. Sélectionnez la flèche déroulante dans la première ligne vide. Dans le menu qui apparaît, sélectionnez la colonne **Propriétaire**.
14. Remplacez le champ **Égal** par Égal à l’utilisateur actuel.
15. Cliquez sur le bouton **OK**.
16. Cliquez sur le bouton **Enregistrer et publier**.

### Tâche n° 3 : ajouter une section Tableaux de bord à l’application Gestion des dépenses des employés
1. Si ce n’est pas déjà fait, connectez-vous à https://make.powerapps.com.
2. Sélectionnez l’environnement dans lequel vous avez importé la solution Note de frais en haut à droite si elle n’est pas déjà sélectionnée.
3. Dans le volet de navigation de gauche, sélectionnez **Solutions.**
4. Ouvrez la solution Note de frais.
5. Sélectionner **les applications**.
6. Recherchez l’application Gestion des dépenses des employés.
7. Cliquez sur les **points de suspension verticaux**, puis sélectionnez **Modifier** dans le menu qui s’affiche.
8. Sélectionnez le bouton **Ajouter une page**.
9. Sélectionnez **Tableau de bord**.
10. Explorez les tableaux de bord système disponibles par défaut. Lorsque vous êtes prêt, sélectionnez l’un des tableaux de bord que vous souhaitez ajouter à votre application.
11. Sélectionnez **Ajouter**.
12. Survolez le groupe Notes de frais sous Navigation.
13. Sélectionnez les **points de suspension**. Dans le menu qui s’affiche, sélectionnez **Nouveau groupe**.
14. Avec le nouveau groupe sélectionné, modifiez le titre en **Tableaux de bord.**
15. Sélectionnez les points de suspension à côté des tableaux de bord et choisissez **Déplacer vers le haut.** Le tableau de bord se trouve désormais au-dessus des notes de frais.
16. Recherchez et sélectionnez le tableau de bord système que vous avez ajouté précédemment dans la tâche.
17. Sélectionnez les points de suspension. Dans le menu qui s’affiche, sélectionnez **Déplacer vers le haut.**
18. Répétez l’étape 17 pour déplacer le tableau de bord système au-dessus de la vue Notes de frais.
19. Répétez l’étape 17 une fois de plus pour déplacer le tableau de bord système dans le groupe Tableaux de bord.
20. Sélectionnez le bouton **Enregistrer**.
21. Une fois la sauvegarde terminée, cliquez sur le bouton **Publier**.

### Tâche n° 4 : ajouter un tableau de bord personnel à l’application Gestion des dépenses des employés
1. Si ce n’est pas déjà fait, connectez-vous à `https://make.powerapps.com`.
2. Sélectionnez l’environnement dans lequel vous avez importé la solution Note de frais en haut à droite si elle n’est pas déjà sélectionnée.
3. Dans le volet de navigation de gauche, sélectionnez **Solutions.**
4. Ouvrez la solution Note de frais.
5. Sélectionner **les applications**.
6. Recherchez l’application pilotée par modèle Gestion des dépenses des employés.
7. Sélectionnez les **points de suspension verticaux**. Dans le menu qui s’affiche, sélectionnez **Lecture**.
8. Sous le groupe Tableaux de bord, sélectionnez le tableau de bord système que vous avez ajouté dans la tâche 3.
9. Sélectionnez le bouton **Nouveau**.
10. Dans le menu qui s’affiche, sélectionnez **Tableau de bord Dynamics 365.**
11. Choisissez **un tableau de bord standard à 2 colonnes.**
12. Cliquez sur le bouton **Créer**.
13. Modifiez le nom du tableau de bord en *`Expense Report Dashboard`*.
14. Sélectionnez l’**icône Liste** dans le coin supérieur gauche.
15. Configurez la liste comme suit :
    - Type d’enregistrement : notes de frais
    - Affichage : notes de frais dues aujourd’hui.
16. Cliquez sur le bouton **Ajouter**.
17. Sélectionnez l’**icône Liste** dans le coin supérieur droit.
18. Configurez la liste comme suit :
    - Type d’enregistrement : notes de frais
    - Affichage : mes notes de frais actives
19. Cliquez sur le bouton **Ajouter**.
20. Sélectionnez l’**icône Liste** dans le coin inférieur gauche.
21. Configurez la liste comme suit :
    - Type d’enregistrement : lignes de dépenses
    - Affichage : mes lignes de dépenses actives
22. Cliquez sur le bouton **Ajouter**.
23. Sélectionnez l’**icône Liste** dans le coin inférieur droit.
24. Configurez la liste comme suit :
    - Type d’enregistrement : contacts
    - Affichage : contacts actifs
25. Cliquez sur le bouton **Ajouter**.
26. Sélectionnez le bouton **Enregistrer** dans le coin supérieur gauche.
27. Une fois le tableau de bord enregistré, sélectionnez le bouton **Fermer**.
28. Vous êtes alors redirigé vers le tableau de bord Notes de frais.
29. Sur la barre de commandes située en haut, sélectionnez **Définir comme valeur par défaut**.
