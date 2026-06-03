| Faculté | Polydisciplinaire | de Khouribga |
| ------- | ----------------- | ------------ |
|         | Support de        | Cours        |
DevOps
|     | S8 - Master | SIIA |
| --- | ----------- | ---- |
Prof : I. AATTOURI
|     | Année Universitaire | 2025–2026 |
| --- | ------------------- | --------- |

Table des matières
1 Introduction et Culture DevOps 3
1.1 Historique et Contexte . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3
1.2 Définition et Philosophie . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3
1.2.1 Les trois piliers du DevOps . . . . . . . . . . . . . . . . . . . . . . 3
1.3 Le Cycle de Vie DevOps (CALMS) . . . . . . . . . . . . . . . . . . . . . . 3
1.4 Le Pipeline DevOps . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4
1.5 Avantages du DevOps . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4
2 Gestion de Versions et Collaboration avec Git 5
2.1 Introduction à Git . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5
2.2 Installation et Configuration initiale . . . . . . . . . . . . . . . . . . . . . . 5
2.3 Commandes Fondamentales . . . . . . . . . . . . . . . . . . . . . . . . . . 6
2.3.1 Initialisation et Clonage . . . . . . . . . . . . . . . . . . . . . . . . 6
2.3.2 Suivre les Fichiers (Staging) . . . . . . . . . . . . . . . . . . . . . . 6
2.3.3 Valider les Modifications (Commit) . . . . . . . . . . . . . . . . . . 7
2.3.4 Consulter l’Historique . . . . . . . . . . . . . . . . . . . . . . . . . 7
2.3.5 Gestion des Branches . . . . . . . . . . . . . . . . . . . . . . . . . . 8
2.3.6 Fusion et Rebase . . . . . . . . . . . . . . . . . . . . . . . . . . . . 8
2.3.7 Interaction avec le Depot Distant . . . . . . . . . . . . . . . . . . . 9
2.3.8 Annuler des Modifications . . . . . . . . . . . . . . . . . . . . . . . 10
2.3.9 Etiquettes (Tags) . . . . . . . . . . . . . . . . . . . . . . . . . . . . 11
2.4 Stratégies de Branchement . . . . . . . . . . . . . . . . . . . . . . . . . . . 11
2.4.1 Git Flow . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 11
2.4.2 Trunk-Based Development . . . . . . . . . . . . . . . . . . . . . . . 12
2.5 Fichier .gitignore . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 12
3 Intégration Continue (CI) 14
3.1 Définition et Principes . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 14
3.2 Jenkins . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 14
3.2.1 Présentation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 14
3.2.2 Installation de Jenkins . . . . . . . . . . . . . . . . . . . . . . . . . 14
3.2.3 Gestion de Jenkins via CLI . . . . . . . . . . . . . . . . . . . . . . 15
3.2.4 Jenkinsfile – Pipeline Déclaratif . . . . . . . . . . . . . . . . . . . . 16
3.2.5 Gestion des Credentials Jenkins . . . . . . . . . . . . . . . . . . . . 19
3.2.6 GitHub Actions – Alternative à Jenkins . . . . . . . . . . . . . . . 20
4 Livraison et Déploiement Continu (CD) 22
4.1 Définitions . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 22
4.2 Stratégies de Déploiement . . . . . . . . . . . . . . . . . . . . . . . . . . . 22
1

Module DevOps S8-SIIA
4.2.1 Blue-Green Deployment . . . . . . . . . . . . . . . . . . . . . . . . 22
4.2.2 Canary Deployment . . . . . . . . . . . . . . . . . . . . . . . . . . . 22
4.2.3 Rolling Update . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 22
4.2.4 Feature Flags . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 22
5 Conteneurisation avec Docker 23
5.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 23
5.2 Installation de Docker . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 23
5.3 Gestion des Images . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 24
5.4 Gestion des Conteneurs . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 25
5.5 Le Dockerfile . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 27
5.5.1 Construction d’Images . . . . . . . . . . . . . . . . . . . . . . . . . 29
5.6 Réseaux Docker . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 30
5.7 Volumes Docker . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 31
5.8 Docker Compose . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 31
6 Orchestration avec Kubernetes 35
6.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 35
6.2 Architecture de Kubernetes . . . . . . . . . . . . . . . . . . . . . . . . . . 35
6.2.1 Composants du Plan de Contrôle (Control Plane) . . . . . . . . . . 35
6.2.2 Composants des Nœuds Workers . . . . . . . . . . . . . . . . . . . 35
6.3 Installation et Configuration (kubectl) . . . . . . . . . . . . . . . . . . . . 35
6.4 Ressources Fondamentales . . . . . . . . . . . . . . . . . . . . . . . . . . . 36
6.4.1 Namespace . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 36
6.4.2 Pod . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 37
6.4.3 Deployment . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 39
6.4.4 Service . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 41
6.4.5 ConfigMap et Secret . . . . . . . . . . . . . . . . . . . . . . . . . . 42
6.4.6 PersistentVolume et PersistentVolumeClaim . . . . . . . . . . . . . 43
6.4.7 Ingress . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 44
6.5 Commandes Générales kubectl . . . . . . . . . . . . . . . . . . . . . . . . . 45
6.6 Helm – Gestionnaire de Paquets Kubernetes . . . . . . . . . . . . . . . . . 46
7 Infrastructure as Code 48
7.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 48
7.2 Terraform . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 48
7.2.1 Présentation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 48
7.2.2 Installation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 48
7.2.3 Commandes Terraform . . . . . . . . . . . . . . . . . . . . . . . . . 49
7.2.4 Exemple de Configuration Terraform . . . . . . . . . . . . . . . . . 50
7.3 Ansible . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 52
7.3.1 Présentation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 52
7.3.2 Installation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 52
7.3.3 Commandes Ansible . . . . . . . . . . . . . . . . . . . . . . . . . . 52
2

| Chapitre     |            | 1   |             |     |        |     |
| ------------ | ---------- | --- | ----------- | --- | ------ | --- |
| Introduction |            |     | et Culture  |     | DevOps |     |
| 1.1          | Historique |     | et Contexte |     |        |     |
Le terme DevOps est une contraction de Development (développement) et Operations
(exploitation). Il désigne un ensemble de pratiques, de méthodes et d’outils visant à amé-
liorer la collaboration entre les équipes de développement logiciel et les équipes d’exploi-
tation informatique.
Avant DevOps, les organisations travaillaient en silos : les développeurs écrivaient du code
et le transmettaient aux équipes opérationnelles qui se chargeaient de le déployer et de
le maintenir en production. Cette approche générait de nombreux problèmes : conflits de
responsabilité, délais de mise en production longs, instabilité des systèmes.
| 1.2 | Définition | et  | Philosophie |     |     |     |
| --- | ---------- | --- | ----------- | --- | --- | --- |
Définition : DevOps est une approche culturelle, organisationnelle et technique qui
vise à unifier le développement logiciel (Dev) et l’administration des systèmes infor-
matiques (Ops) afin de livrer des applications de manière continue, fiable et rapide.
| 1.2.1 | Les trois | piliers | du DevOps |     |     |     |
| ----- | --------- | ------- | --------- | --- | --- | --- |
1. Culture : collaboration, partage de responsabilités, apprentissage continu.
2. Automatisation : réduction des tâches manuelles répétitives.
3. Mesure : collecte de métriques, amélioration continue basée sur les données.
| 1.3       | Le Cycle | de     | Vie DevOps                | (CALMS) |           |     |
| --------- | -------- | ------ | ------------------------- | ------- | --------- | --- |
| Le modèle | CALMS    | résume | les valeurs fondamentales |         | du DevOps | :   |
3

| Module DevOps  |                 |                |             |                  |             |                |                |                   | S8-SIIA     |
| -------------- | --------------- | -------------- | ----------- | ---------------- | ----------- | -------------- | -------------- | ----------------- | ----------- |
|                |                 | Lettre         |             | Signification    |             |                |                |                   |             |
|                |                 | C              |             | Culture          |             | (collaboration |                | entre             | Dev et Ops) |
|                |                 | A              |             | Automatisation   |             |                | (des           | processus         | répétitifs) |
|                |                 | L              |             | Lean             | (réduction  |                | du             | gaspillage)       |             |
|                |                 | M              |             | Measurement      |             |                | (métriques     | et                | feedback)   |
|                |                 | S              |             | Sharing          |             | (partage       | des            | connaissances)    |             |
| 1.4            | Le Pipeline     |                |             | DevOps           |             |                |                |                   |             |
| Le cycle       | de vie          | DevOps         | comprend    |                  | les         | phases         | suivantes      | :                 |             |
| 1. Plan        | : définition    |                | des         | besoins          | et          | des            | objectifs.     |                   |             |
| 2. Code        | : développement |                |             | du               | logiciel.   |                |                |                   |             |
| 3. Build       | : compilation   |                |             | et assemblage    |             | du             | code.          |                   |             |
| 4. Test        | : vérification  |                | automatique |                  |             | de la          | qualité.       |                   |             |
| 5. Release     | :               | préparation    |             | du               | livrable.   |                |                |                   |             |
| 6. Deploy      | :               | déploiement    |             | en               | production. |                |                |                   |             |
| 7. Operate     |                 | : gestion      | de          | l’infrastructure |             |                | en production. |                   |             |
| 8. Monitor     |                 | : surveillance |             | et               | collecte    | de             | métriques.     |                   |             |
| 1.5            | Avantages       |                | du          | DevOps           |             |                |                |                   |             |
| — Réduction    |                 | du délai       | de          | mise             | sur         | le marché      |                | (time-to-market). |             |
| — Amélioration |                 | de             | la qualité  |                  | logicielle. |                |                |                   |             |
| — Meilleure    |                 | stabilité      | des         | systèmes         |             | en production. |                |                   |             |
| — Réduction    |                 | des            | coûts       | opérationnels.   |             |                |                |                   |             |
| — Augmentation |                 |                | de la       | satisfaction     |             | client.        |                |                   |             |
4

| Chapitre |              |     | 2        |       |     |     |               |     |
| -------- | ------------ | --- | -------- | ----- | --- | --- | ------------- | --- |
| Gestion  |              | de  | Versions |       |     | et  | Collaboration |     |
| avec     | Git          |     |          |       |     |     |               |     |
| 2.1      | Introduction |     |          | à Git |     |     |               |     |
Git est un système de gestion de versions distribué créé par Linus Torvalds en 2005. Il
permet de suivre les modifications apportées au code source, de collaborer efficacement
| et de gérer | plusieurs |     | versions | d’un projet | simultanément. |     |     |     |
| ----------- | --------- | --- | -------- | ----------- | -------------- | --- | --- | --- |
Dépôt (Repository) : répertoire versionné contenant l’ensemble du code source et
| l’historique |              | complet  | des | modifications.   |     |     |          |     |
| ------------ | ------------ | -------- | --- | ---------------- | --- | --- | -------- | --- |
| 2.2          | Installation |          |     | et Configuration |     |     | initiale |     |
| # Debian     |              | / Ubuntu |     |                  |     |     |          |     |
1
| sudo | apt-get | update |     | && sudo | apt-get |     | install | -y git |
| ---- | ------- | ------ | --- | ------- | ------- | --- | ------- | ------ |
2
3
| # CentOS |     | / RHEL |     |     |     |     |     |     |
| -------- | --- | ------ | --- | --- | --- | --- | --- | --- |
4
| sudo | yum | install | -y  | git |     |     |     |     |
| ---- | --- | ------- | --- | --- | --- | --- | --- | --- |
5
6
| # macOS | (avec | Homebrew) |     |     |     |     |     |     |
| ------- | ----- | --------- | --- | --- | --- | --- | --- | --- |
7
| brew | install | git |     |     |     |     |     |     |
| ---- | ------- | --- | --- | --- | --- | --- | --- | --- |
8
|           |     |        |               | Listing | 2.1 – Installation |     | de  | Git |
| --------- | --- | ------ | ------------- | ------- | ------------------ | --- | --- | --- |
| # Definir |     | le nom | d’utilisateur |         |                    |     |     |     |
1
| git config |     | --global |     | user.name | "Prenom |     | NOM" |     |
| ---------- | --- | -------- | --- | --------- | ------- | --- | ---- | --- |
2
3
| # Definir |     | l’adresse |     | email |     |     |     |     |
| --------- | --- | --------- | --- | ----- | --- | --- | --- | --- |
4
| git config |     | --global |     | user.email |     | "prenom.nom@exemple.com" |     |     |
| ---------- | --- | -------- | --- | ---------- | --- | ------------------------ | --- | --- |
5
6
| # Definir |     | l’editeur |     | par defaut |     |     |     |     |
| --------- | --- | --------- | --- | ---------- | --- | --- | --- | --- |
7
| git config |     | --global |     | core.editor |     | vim |     |     |
| ---------- | --- | -------- | --- | ----------- | --- | --- | --- | --- |
8
9
| 10 # Definir |     | la branche |     | principale         |     | par | defaut |     |
| ------------ | --- | ---------- | --- | ------------------ | --- | --- | ------ | --- |
| git config   |     | --global   |     | init.defaultBranch |     |     | main   |     |
11
5

| Module DevOps |     |     |     |     |     |     |     | S8-SIIA |
| ------------- | --- | --- | --- | --- | --- | --- | --- | ------- |
12
| 13 # Afficher |     | la configuration |     |     | actuelle |     |     |     |
| ------------- | --- | ---------------- | --- | --- | -------- | --- | --- | --- |
| git config    |     | --list           |     |     |          |     |     |     |
14
15
| 16 # Afficher |     | un parametre |     |     | specifique |     |     |     |
| ------------- | --- | ------------ | --- | --- | ---------- | --- | --- | --- |
| git config    |     | user.name    |     |     |            |     |     |     |
17
|                      |     |     | Listing | 2.2           | – Configuration |       | globale | de Git |
| -------------------- | --- | --- | ------- | ------------- | --------------- | ----- | ------- | ------ |
| 2.3 Commandes        |     |     |         | Fondamentales |                 |       |         |        |
| 2.3.1 Initialisation |     |     |         | et            | Clonage         |       |         |        |
| # Initialiser        |     | un  | nouveau |               | depot           | local |         |        |
1
| 2 git init |     |     |     |     |     |     |     |     |
| ---------- | --- | --- | --- | --- | --- | --- | --- | --- |
3
| # Initialiser |     | un  | depot |     | avec un | nom | de repertoire |     |
| ------------- | --- | --- | ----- | --- | ------- | --- | ------------- | --- |
4
| git init | mon-projet |     |     |     |     |     |     |     |
| -------- | ---------- | --- | --- | --- | --- | --- | --- | --- |
5
6
| # Cloner | un  | depot | distant |     | (HTTPS) |     |     |     |
| -------- | --- | ----- | ------- | --- | ------- | --- | --- | --- |
7
| git clone |     | https://github.com/utilisateur/depot.git |     |     |     |     |     |     |
| --------- | --- | ---------------------------------------- | --- | --- | --- | --- | --- | --- |
8
9
| # Cloner | avec | SSH |     |     |     |     |     |     |
| -------- | ---- | --- | --- | --- | --- | --- | --- | --- |
10
| git clone |     | git@github.com:utilisateur/depot.git |     |     |     |     |     |     |
| --------- | --- | ------------------------------------ | --- | --- | --- | --- | --- | --- |
11
12
| # Cloner | dans | un  | repertoire |     | specifique |     |     |     |
| -------- | ---- | --- | ---------- | --- | ---------- | --- | --- | --- |
13
git clone https://github.com/utilisateur/depot.git mon-dossier
14
15
| 16 # Cloner | une | branche |     | specifique |     |     |     |     |
| ----------- | --- | ------- | --- | ---------- | --- | --- | --- | --- |
git clone -b develop https://github.com/utilisateur/depot.git
17
18
| 19 # Cloner | sans | l’historique |     |                                          | complet |     | (shallow | clone) |
| ----------- | ---- | ------------ | --- | ---------------------------------------- | ------- | --- | -------- | ------ |
| git clone   |      | --depth      | 1   | https://github.com/utilisateur/depot.git |         |     |          |        |
20
|              |     | Listing |          | 2.3   | – Initialisation |     | et clonage | d’un depot |
| ------------ | --- | ------- | -------- | ----- | ---------------- | --- | ---------- | ---------- |
| 2.3.2 Suivre |     | les     | Fichiers |       | (Staging)        |     |            |            |
| 1 # Afficher |     | l’etat  | du       | depot |                  |     |            |            |
| git status   |     |         |          |       |                  |     |            |            |
2
3
| 4 # Afficher |     | l’etat | en  | format | court |     |     |     |
| ------------ | --- | ------ | --- | ------ | ----- | --- | --- | --- |
| git status   |     | -s     |     |        |       |     |     |     |
5
6
| # Ajouter |     | un fichier |     | specifique |     | a   | la zone | de transit |
| --------- | --- | ---------- | --- | ---------- | --- | --- | ------- | ---------- |
7
| 8 git add | fichier.txt |     |     |     |     |     |     |     |
| --------- | ----------- | --- | --- | --- | --- | --- | --- | --- |
9
| # Ajouter |     | tous | les | fichiers | modifies |     |     |     |
| --------- | --- | ---- | --- | -------- | -------- | --- | --- | --- |
10
| 11 git add | .   |     |     |     |     |     |     |     |
| ---------- | --- | --- | --- | --- | --- | --- | --- | --- |
12
6

| Module DevOps |     |          |          |     |       |     |           | S8-SIIA |
| ------------- | --- | -------- | -------- | --- | ----- | --- | --------- | ------- |
| # Ajouter     |     | tous les | fichiers |     | d’une |     | extension |         |
13
| 14 git add | *.java |     |     |     |     |     |     |     |
| ---------- | ------ | --- | --- | --- | --- | --- | --- | --- |
15
| # Ajouter |     | de maniere |     | interactive |     | (selectif) |     |     |
| --------- | --- | ---------- | --- | ----------- | --- | ---------- | --- | --- |
16
| 17 git add | -p  |     |     |     |     |     |     |     |
| ---------- | --- | --- | --- | --- | --- | --- | --- | --- |
18
| # Retirer |     | un fichier |     | de la | zone | de  | transit |     |
| --------- | --- | ---------- | --- | ----- | ---- | --- | ------- | --- |
19
| git restore |     | --staged |     | fichier.txt |     |     |     |     |
| ----------- | --- | -------- | --- | ----------- | --- | --- | --- | --- |
20
21
| # Ancienne |     | syntaxe | equivalente |     |     |     |     |     |
| ---------- | --- | ------- | ----------- | --- | --- | --- | --- | --- |
22
| git reset |     | HEAD fichier.txt |     |     |     |     |     |     |
| --------- | --- | ---------------- | --- | --- | --- | --- | --- | --- |
23
|         |         |        | Listing       | 2.4 – | Zone    | de transit | (staging | area) |
| ------- | ------- | ------ | ------------- | ----- | ------- | ---------- | -------- | ----- |
| 2.3.3   | Valider | les    | Modifications |       |         | (Commit)   |          |       |
| # Creer | un      | commit | avec          | un    | message |            |          |       |
1
git commit -m "feat: ajout de la fonctionnalite de connexion"
2
3
| # Ajouter |     | et committer |     | en  | une | seule | commande |     |
| --------- | --- | ------------ | --- | --- | --- | ----- | -------- | --- |
4
| git commit |     | -am "fix: |     | correction |     | du  | bug d’authentification" |     |
| ---------- | --- | --------- | --- | ---------- | --- | --- | ----------------------- | --- |
5
6
| # Amender |     | le dernier |     | commit | (message |     | ou contenu) |     |
| --------- | --- | ---------- | --- | ------ | -------- | --- | ----------- | --- |
7
| git commit |     | --amend | -m  | "feat: |     | nouveau | message" |     |
| ---------- | --- | ------- | --- | ------ | --- | ------- | -------- | --- |
8
9
| # Amender |     | sans changer |     | le  | message |     |     |     |
| --------- | --- | ------------ | --- | --- | ------- | --- | --- | --- |
10
| git commit |     | --amend | --no-edit |     |     |     |     |     |
| ---------- | --- | ------- | --------- | --- | --- | --- | --- | --- |
11
12
| 13 # Commit | vide | (utile        |     | pour | CI)         |     |     |     |
| ----------- | ---- | ------------- | --- | ---- | ----------- | --- | --- | --- |
| git commit  |      | --allow-empty |     |      | -m "trigger |     | CI" |     |
14
|            |           |              | Listing      | 2.5 | – Commandes |     | de commit |     |
| ---------- | --------- | ------------ | ------------ | --- | ----------- | --- | --------- | --- |
| 2.3.4      | Consulter |              | l’Historique |     |             |     |           |     |
| # Afficher |           | l’historique |              | des | commits     |     |           |     |
1
| git log |     |     |     |     |     |     |     |     |
| ------- | --- | --- | --- | --- | --- | --- | --- | --- |
2
3
| 4 # Afficher |           | l’historique |     | en  | une | ligne | par commit |     |
| ------------ | --------- | ------------ | --- | --- | --- | ----- | ---------- | --- |
| git log      | --oneline |              |     |     |     |       |            |     |
5
6
| 7 # Afficher |           | avec | graphe  | des | branches |     |     |     |
| ------------ | --------- | ---- | ------- | --- | -------- | --- | --- | --- |
| git log      | --oneline |      | --graph |     | --all    |     |     |     |
8
9
| # Afficher |     | les n | derniers |     | commits |     |     |     |
| ---------- | --- | ----- | -------- | --- | ------- | --- | --- | --- |
10
| git log | -n  | 5   |     |     |     |     |     |     |
| ------- | --- | --- | --- | --- | --- | --- | --- | --- |
11
12
| # Filtrer |     | par auteur |     |     |     |     |     |     |
| --------- | --- | ---------- | --- | --- | --- | --- | --- | --- |
13
| 14 git log | --author="AATTOURI" |     |     |     |     |     |     |     |
| ---------- | ------------------- | --- | --- | --- | --- | --- | --- | --- |
15
| # Filtrer |     | par date |     |     |     |     |     |     |
| --------- | --- | -------- | --- | --- | --- | --- | --- | --- |
16
7

| Module DevOps |                      |     |     |     |     |                      |     |     |     | S8-SIIA |
| ------------- | -------------------- | --- | --- | --- | --- | -------------------- | --- | --- | --- | ------- |
| git log       | --since="2024-01-01" |     |     |     |     | --until="2024-12-31" |     |     |     |         |
17
18
| # Afficher |     | les | modifications |     |     | d’un | commit |     |     |     |
| ---------- | --- | --- | ------------- | --- | --- | ---- | ------ | --- | --- | --- |
19
| git show | <hash-commit> |     |     |     |     |     |     |     |     |     |
| -------- | ------------- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
20
21
| # Afficher |     | les | differences |     |     | non committees |     |     |     |     |
| ---------- | --- | --- | ----------- | --- | --- | -------------- | --- | --- | --- | --- |
22
| git diff |     |     |     |     |     |     |     |     |     |     |
| -------- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
23
24
| 25 # Afficher |          | les    | differences |     |     | entre | la zone | de  | transit | et le |
| ------------- | -------- | ------ | ----------- | --- | --- | ----- | ------- | --- | ------- | ----- |
| dernier       |          | commit |             |     |     |       |         |     |         |       |
| git diff      | --staged |        |             |     |     |       |         |     |         |       |
26
|          |         |          | Listing |          | 2.6 – | Consultation | de  | l’historique |     |     |
| -------- | ------- | -------- | ------- | -------- | ----- | ------------ | --- | ------------ | --- | --- |
| 2.3.5    | Gestion |          | des     | Branches |       |              |     |              |     |     |
| # Lister | les     | branches |         | locales  |       |              |     |              |     |     |
1
| git branch |     |     |     |     |     |     |     |     |     |     |
| ---------- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
2
3
| # Lister | toutes |     | les | branches |     | (locales |     | et distantes) |     |     |
| -------- | ------ | --- | --- | -------- | --- | -------- | --- | ------------- | --- | --- |
4
| git branch |     | -a  |     |     |     |     |     |     |     |     |
| ---------- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
5
6
| # Creer | une | nouvelle |     | branche |     |     |     |     |     |     |
| ------- | --- | -------- | --- | ------- | --- | --- | --- | --- | --- | --- |
7
| git branch |     | feature/ma-fonctionnalite |     |     |     |     |     |     |     |     |
| ---------- | --- | ------------------------- | --- | --- | --- | --- | --- | --- | --- | --- |
8
9
| # Basculer |     | sur | une | branche |     | existante |     |     |     |     |
| ---------- | --- | --- | --- | ------- | --- | --------- | --- | --- | --- | --- |
10
| git checkout |     | develop |     |     |     |     |     |     |     |     |
| ------------ | --- | ------- | --- | --- | --- | --- | --- | --- | --- | --- |
11
| git switch |     | develop |     |     |     | # nouvelle |     | syntaxe | recommandee |     |
| ---------- | --- | ------- | --- | --- | --- | ---------- | --- | ------- | ----------- | --- |
12
13
| # Creer | et  | basculer |     | sur | une | nouvelle | branche |     |     |     |
| ------- | --- | -------- | --- | --- | --- | -------- | ------- | --- | --- | --- |
14
| git checkout |     | -b  | feature/ma-fonctionnalite |     |     |     |     |     |     |     |
| ------------ | --- | --- | ------------------------- | --- | --- | --- | --- | --- | --- | --- |
15
16 git switch -c feature/ma-fonctionnalite # nouvelle syntaxe
17
| # Renommer |     | une | branche |     |     |     |     |     |     |     |
| ---------- | --- | --- | ------- | --- | --- | --- | --- | --- | --- | --- |
18
| git branch |     | -m  | ancien-nom |     | nouveau-nom |     |     |     |     |     |
| ---------- | --- | --- | ---------- | --- | ----------- | --- | --- | --- | --- | --- |
19
20
| # Supprimer |     | une | branche |     | locale |     |     |     |     |     |
| ----------- | --- | --- | ------- | --- | ------ | --- | --- | --- | --- | --- |
21
| git branch |     | -d  | feature/ma-fonctionnalite |     |     |     |     |     |     |     |
| ---------- | --- | --- | ------------------------- | --- | --- | --- | --- | --- | --- | --- |
22
23
| # Forcer | la  | suppression |     |     | d’une | branche |     | non | merged |     |
| -------- | --- | ----------- | --- | --- | ----- | ------- | --- | --- | ------ | --- |
24
| git branch |     | -D  | feature/ma-fonctionnalite |     |     |     |     |     |     |     |
| ---------- | --- | --- | ------------------------- | --- | --- | --- | --- | --- | --- | --- |
25
26
| 27 # Supprimer |        | une | branche  |     | distante                  |     |     |     |     |     |
| -------------- | ------ | --- | -------- | --- | ------------------------- | --- | --- | --- | --- | --- |
| git push       | origin |     | --delete |     | feature/ma-fonctionnalite |     |     |     |     |     |
28
|             |        |     |         | Listing | 2.7  | – Gestion  | des | branches |     |     |
| ----------- | ------ | --- | ------- | ------- | ---- | ---------- | --- | -------- | --- | --- |
| 2.3.6       | Fusion | et  | Rebase  |         |      |            |     |          |     |     |
| # Fusionner |        | une | branche |         | dans | la branche |     | courante |     |     |
1
| git merge |     | feature/ma-fonctionnalite |     |     |     |     |     |     |     |     |
| --------- | --- | ------------------------- | --- | --- | --- | --- | --- | --- | --- | --- |
2
8

| Module DevOps |     |     |     |     |     |     |     | S8-SIIA |
| ------------- | --- | --- | --- | --- | --- | --- | --- | ------- |
3
| 4 # Fusion | sans | fast-forward |                           |     |     | (conserve | l’historique) |     |
| ---------- | ---- | ------------ | ------------------------- | --- | --- | --------- | ------------- | --- |
| git merge  |      | --no-ff      | feature/ma-fonctionnalite |     |     |           |               |     |
5
6
| 7 # Rebaser |     | la branche |     | courante |     | sur | main |     |
| ----------- | --- | ---------- | --- | -------- | --- | --- | ---- | --- |
| git rebase  |     | main       |     |          |     |     |      |     |
8
9
| # Rebaser |     | interactivement |     |     | les | 3 derniers |     | commits |
| --------- | --- | --------------- | --- | --- | --- | ---------- | --- | ------- |
10
| 11 git rebase |     | -i HEAD~3 |     |     |     |     |     |     |
| ------------- | --- | --------- | --- | --- | --- | --- | --- | --- |
12
| # Abandonner |     | un  | rebase |     | en cours |     |     |     |
| ------------ | --- | --- | ------ | --- | -------- | --- | --- | --- |
13
| 14 git rebase |     | --abort |     |     |     |     |     |     |
| ------------- | --- | ------- | --- | --- | --- | --- | --- | --- |
15
| # Continuer |     | apres | resolution |     |     | de conflit |     |     |
| ----------- | --- | ----- | ---------- | --- | --- | ---------- | --- | --- |
16
| git rebase |     | --continue |     |     |     |     |     |     |
| ---------- | --- | ---------- | --- | --- | --- | --- | --- | --- |
17
18
| # Cherry-pick |     | :   | appliquer |     | un  | commit | specifique |     |
| ------------- | --- | --- | --------- | --- | --- | ------ | ---------- | --- |
19
| git cherry-pick |     |     | <hash-commit> |     |     |     |     |     |
| --------------- | --- | --- | ------------- | --- | --- | --- | --- | --- |
20
|            |             |     |        | Listing  | 2.8      | – Fusion | de branches |     |
| ---------- | ----------- | --- | ------ | -------- | -------- | -------- | ----------- | --- |
| 2.3.7      | Interaction |     | avec   |          | le Depot |          | Distant     |     |
| # Afficher |             | les | depots | distants |          |          |             |     |
1
| 2 git remote |     | -v  |     |     |     |     |     |     |
| ------------ | --- | --- | --- | --- | --- | --- | --- | --- |
3
| # Ajouter |     | un depot |     | distant |     |     |     |     |
| --------- | --- | -------- | --- | ------- | --- | --- | --- | --- |
4
git remote add origin https://github.com/utilisateur/depot.git
5
6
| # Modifier |     | l’URL | d’un | depot |     | distant |     |     |
| ---------- | --- | ----- | ---- | ----- | --- | ------- | --- | --- |
7
git remote set-url origin git@github.com:utilisateur/depot.git
8
9
| # Supprimer |     | un  | depot | distant |     |     |     |     |
| ----------- | --- | --- | ----- | ------- | --- | --- | --- | --- |
10
| git remote |     | remove | origin |     |     |     |     |     |
| ---------- | --- | ------ | ------ | --- | --- | --- | --- | --- |
11
12
| 13 # Recuperer |     | les    | modifications |     |     | sans | merger |     |
| -------------- | --- | ------ | ------------- | --- | --- | ---- | ------ | --- |
| git fetch      |     | origin |               |     |     |      |        |     |
14
15
| 16 # Recuperer |     | toutes |     | les | branches | distantes |     |     |
| -------------- | --- | ------ | --- | --- | -------- | --------- | --- | --- |
| git fetch      |     | --all  |     |     |          |           |     |     |
17
18
| # Tirer | (fetch |     | + merge) |     | la  | branche | courante |     |
| ------- | ------ | --- | -------- | --- | --- | ------- | -------- | --- |
19
| 20 git pull |     |     |     |     |     |     |     |     |
| ----------- | --- | --- | --- | --- | --- | --- | --- | --- |
21
| # Tirer | avec | rebase |     |     |     |     |     |     |
| ------- | ---- | ------ | --- | --- | --- | --- | --- | --- |
22
| 23 git pull | --rebase |     |     |     |     |     |     |     |
| ----------- | -------- | --- | --- | --- | --- | --- | --- | --- |
24
| # Pousser |     | la branche |     | courante |     | vers | le depot | distant |
| --------- | --- | ---------- | --- | -------- | --- | ---- | -------- | ------- |
25
| git push | origin |     | main |     |     |     |     |     |
| -------- | ------ | --- | ---- | --- | --- | --- | --- | --- |
26
27
| # Pousser |     | et configurer |     |     | le  | suivi |     |     |
| --------- | --- | ------------- | --- | --- | --- | ----- | --- | --- |
28
9

| Module DevOps |     |        |     |                           |     |     |     |     | S8-SIIA |
| ------------- | --- | ------ | --- | ------------------------- | --- | --- | --- | --- | ------- |
| git push      | -u  | origin |     | feature/ma-fonctionnalite |     |     |     |     |         |
29
30
| # Pousser |     | tous | les | tags |     |     |     |     |     |
| --------- | --- | ---- | --- | ---- | --- | --- | --- | --- | --- |
31
| git push | --tags |     |     |     |     |     |     |     |     |
| -------- | ------ | --- | --- | --- | --- | --- | --- | --- | --- |
32
|           |         |     | Listing       | 2.9           | – Commandes |         | distantes | (remote) |         |
| --------- | ------- | --- | ------------- | ------------- | ----------- | ------- | --------- | -------- | ------- |
| 2.3.8     | Annuler |     | des           | Modifications |             |         |           |          |         |
| # Annuler |         | les | modifications |               | d’un        | fichier |           | (non     | staged) |
1
| git restore |     | fichier.txt |     |     |     |     |     |     |     |
| ----------- | --- | ----------- | --- | --- | --- | --- | --- | --- | --- |
2
3
| # Reinitialiser |     |     | la  | zone | de transit |     |     |     |     |
| --------------- | --- | --- | --- | ---- | ---------- | --- | --- | --- | --- |
4
| git restore |     | --staged |     | fichier.txt |     |     |     |     |     |
| ----------- | --- | -------- | --- | ----------- | --- | --- | --- | --- | --- |
5
6
| # Revenir |     | a un | commit | precedent |     | (soft |     | : conserve | les |
| --------- | --- | ---- | ------ | --------- | --- | ----- | --- | ---------- | --- |
7
modifications)
| git reset |     | --soft | HEAD~1 |     |     |     |     |     |     |
| --------- | --- | ------ | ------ | --- | --- | --- | --- | --- | --- |
8
9
| # Revenir |     | a un | commit | precedent |     | (mixed |     | : defaut) |     |
| --------- | --- | ---- | ------ | --------- | --- | ------ | --- | --------- | --- |
10
| git reset |     | HEAD~1 |     |     |     |     |     |     |     |
| --------- | --- | ------ | --- | --- | --- | --- | --- | --- | --- |
11
12
# Revenir a un commit precedent (hard : perd les modifications)
13
| git reset |     | --hard | HEAD~1 |     |     |     |     |     |     |
| --------- | --- | ------ | ------ | --- | --- | --- | --- | --- | --- |
14
15
| # Creer | un  | commit | annulant |     | un  | commit | precedent |     |     |
| ------- | --- | ------ | -------- | --- | --- | ------ | --------- | --- | --- |
16
| git revert |     | <hash-commit> |     |     |     |     |     |     |     |
| ---------- | --- | ------------- | --- | --- | --- | --- | --- | --- | --- |
17
18
| 19 # Mettre | de  | cote | des | modifications |     |     | temporairement |     |     |
| ----------- | --- | ---- | --- | ------------- | --- | --- | -------------- | --- | --- |
| git stash   |     |      |     |               |     |     |                |     |     |
20
21
| 22 # Mettre | de  | cote | avec        | un  | nom |       |     |         |     |
| ----------- | --- | ---- | ----------- | --- | --- | ----- | --- | ------- | --- |
| git stash   |     | push | -m "travail |     | en  | cours | sur | feature | X"  |
23
24
| # Lister | les | stash |     |     |     |     |     |     |     |
| -------- | --- | ----- | --- | --- | --- | --- | --- | --- | --- |
25
| 26 git stash |     | list |     |     |     |     |     |     |     |
| ------------ | --- | ---- | --- | --- | --- | --- | --- | --- | --- |
27
| # Appliquer |     | le  | dernier |     | stash |     |     |     |     |
| ----------- | --- | --- | ------- | --- | ----- | --- | --- | --- | --- |
28
| 29 git stash |     | apply |     |     |     |     |     |     |     |
| ------------ | --- | ----- | --- | --- | --- | --- | --- | --- | --- |
30
| # Appliquer |     | un  | stash | specifique |     |     |     |     |     |
| ----------- | --- | --- | ----- | ---------- | --- | --- | --- | --- | --- |
31
| git stash |     | apply | stash@{2} |     |     |     |     |     |     |
| --------- | --- | ----- | --------- | --- | --- | --- | --- | --- | --- |
32
33
| # Appliquer |     | et  | supprimer |     | le dernier |     | stash |     |     |
| ----------- | --- | --- | --------- | --- | ---------- | --- | ----- | --- | --- |
34
| git stash |     | pop |     |     |     |     |     |     |     |
| --------- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
35
36
| # Supprimer |     | un  | stash |     |     |     |     |     |     |
| ----------- | --- | --- | ----- | --- | --- | --- | --- | --- | --- |
37
| git stash |     | drop | stash@{0} |     |     |     |     |     |     |
| --------- | --- | ---- | --------- | --- | --- | --- | --- | --- | --- |
38
39
| # Supprimer |     | tous | les | stash |     |     |     |     |     |
| ----------- | --- | ---- | --- | ----- | --- | --- | --- | --- | --- |
40
| git stash |     | clear |     |     |     |     |     |     |     |
| --------- | --- | ----- | --- | --- | --- | --- | --- | --- | --- |
41
10

| Module DevOps |            |         |     |        |            |     | S8-SIIA         |
| ------------- | ---------- | ------- | --- | ------ | ---------- | --- | --------------- |
|               |            | Listing |     | 2.10 – | Annulation |     | et restauration |
| 2.3.9         | Etiquettes | (Tags)  |     |        |            |     |                 |
| # Creer       | un tag     | leger   |     |        |            |     |                 |
1
| git tag | v1.0.0 |     |     |     |     |     |     |
| ------- | ------ | --- | --- | --- | --- | --- | --- |
2
3
| # Creer | un tag | annote | (recommande) |     |     |     |     |
| ------- | ------ | ------ | ------------ | --- | --- | --- | --- |
4
| git tag | -a v1.0.0 |     | -m "Version |     | 1.0.0 |     | stable" |
| ------- | --------- | --- | ----------- | --- | ----- | --- | ------- |
5
6
| # Tagger | un commit |     | specifique |     |     |     |     |
| -------- | --------- | --- | ---------- | --- | --- | --- | --- |
7
| git tag | -a v0.9.0 |     | <hash-commit> |     |     |     |     |
| ------- | --------- | --- | ------------- | --- | --- | --- | --- |
8
9
| 10 # Lister | les tags |     |     |     |     |     |     |
| ----------- | -------- | --- | --- | --- | --- | --- | --- |
| git tag     |          |     |     |     |     |     |     |
11
12
| 13 # Afficher | les    | details |     | d’un | tag |     |     |
| ------------- | ------ | ------- | --- | ---- | --- | --- | --- |
| git show      | v1.0.0 |         |     |      |     |     |     |
14
15
| # Pousser | un tag | specifique |     |     |     |     |     |
| --------- | ------ | ---------- | --- | --- | --- | --- | --- |
16
| 17 git push | origin | v1.0.0 |     |     |     |     |     |
| ----------- | ------ | ------ | --- | --- | --- | --- | --- |
18
| # Pousser | tous | les | tags |     |     |     |     |
| --------- | ---- | --- | ---- | --- | --- | --- | --- |
19
| 20 git push | origin | --tags |     |     |     |     |     |
| ----------- | ------ | ------ | --- | --- | --- | --- | --- |
21
| # Supprimer | un  | tag | local |     |     |     |     |
| ----------- | --- | --- | ----- | --- | --- | --- | --- |
22
| 23 git tag | -d v1.0.0 |     |     |     |     |     |     |
| ---------- | --------- | --- | --- | --- | --- | --- | --- |
24
| # Supprimer | un  | tag | distant |     |     |     |     |
| ----------- | --- | --- | ------- | --- | --- | --- | --- |
25
| git push | origin | --delete |     | v1.0.0 |     |     |     |
| -------- | ------ | -------- | --- | ------ | --- | --- | --- |
26
|                |          |     | Listing        | 2.11 | –   | Gestion | des tags |
| -------------- | -------- | --- | -------------- | ---- | --- | ------- | -------- |
| 2.4 Stratégies |          |     | de Branchement |      |     |         |          |
| 2.4.1          | Git Flow |     |                |      |     |         |          |
Git Flow est une stratégie de branchement populaire qui définit un modèle strict de
| branches    | :          |               |      |               |             |                  |     |
| ----------- | ---------- | ------------- | ---- | ------------- | ----------- | ---------------- | --- |
| — main      | : contient | le code       | de   | production    |             | stable.          |     |
| — develop   | : branche  | d’intégration |      |               | principale. |                  |     |
| — feature/* | : branches |               | pour | les nouvelles |             | fonctionnalités. |     |
— release/* : branches de préparation à la mise en production.
| — hotfix/* | : corrections |     | urgentes |     | en production. |     |     |
| ---------- | ------------- | --- | -------- | --- | -------------- | --- | --- |
11

Module DevOps S8-SIIA
| 1 # Installer |     | git-flow |     |          |     |     |     |
| ------------- | --- | -------- | --- | -------- | --- | --- | --- |
| sudo apt-get  |     | install  |     | git-flow |     |     |     |
2
3
| # Initialiser |     | git-flow |     |     | dans un | depot existant |     |
| ------------- | --- | -------- | --- | --- | ------- | -------------- | --- |
4
| 5 git flow | init |     |     |     |     |     |     |
| ---------- | ---- | --- | --- | --- | --- | --- | --- |
6
| # Demarrer |     | une | nouvelle |     | fonctionnalite |     |     |
| ---------- | --- | --- | -------- | --- | -------------- | --- | --- |
7
| 8 git flow | feature |     | start |     | ma-fonctionnalite |     |     |
| ---------- | ------- | --- | ----- | --- | ----------------- | --- | --- |
9
| # Terminer |     | une | fonctionnalite |     |     |     |     |
| ---------- | --- | --- | -------------- | --- | --- | --- | --- |
10
| git flow | feature |     | finish |     | ma-fonctionnalite |     |     |
| -------- | ------- | --- | ------ | --- | ----------------- | --- | --- |
11
12
| # Demarrer |     | une | release |     |     |     |     |
| ---------- | --- | --- | ------- | --- | --- | --- | --- |
13
| git flow | release |     | start |     | 1.2.0 |     |     |
| -------- | ------- | --- | ----- | --- | ----- | --- | --- |
14
15
| # Terminer |     | une | release |     |     |     |     |
| ---------- | --- | --- | ------- | --- | --- | --- | --- |
16
| git flow | release |     | finish |     | 1.2.0 |     |     |
| -------- | ------- | --- | ------ | --- | ----- | --- | --- |
17
18
| 19 # Demarrer |        | un hotfix |       |                     |     |     |     |
| ------------- | ------ | --------- | ----- | ------------------- | --- | --- | --- |
| git flow      | hotfix |           | start | correction-critique |     |     |     |
20
21
| 22 # Terminer |        | un hotfix |        |     |                     |     |     |
| ------------- | ------ | --------- | ------ | --- | ------------------- | --- | --- |
| git flow      | hotfix |           | finish |     | correction-critique |     |     |
23
|                   |     |     | Listing | 2.12        | – Git | Flow avec l’outil | git-flow |
| ----------------- | --- | --- | ------- | ----------- | ----- | ----------------- | -------- |
| 2.4.2 Trunk-Based |     |     |         | Development |       |                   |          |
Dans cette approche, tous les développeurs committent directement sur une branche
unique (main ou trunk). Les fonctionnalités non finies sont masquées par des feature
flags.
| 2.5 Fichier |     | .gitignore     |     |     |      |     |     |
| ----------- | --- | -------------- | --- | --- | ---- | --- | --- |
| # Fichiers  |     | de compilation |     |     | Java |     |     |
1
2 *.class
*.jar
3
target/
4
5
| # Environnements |     |     | virtuels |     | Python |     |     |
| ---------------- | --- | --- | -------- | --- | ------ | --- | --- |
6
venv/
7
__pycache__/
8
9 *.pyc
10
| # Variables |     | d’environnement |     |     |     |     |     |
| ----------- | --- | --------------- | --- | --- | --- | --- | --- |
11
12 .env
.env.local
13
14
| # Fichiers |     | de l’IDE |     |     |     |     |     |
| ---------- | --- | -------- | --- | --- | --- | --- | --- |
15
16 .idea/
12

| Module DevOps |     |     |     |     | S8-SIIA |
| ------------- | --- | --- | --- | --- | ------- |
.vscode/
17
18 *.swp
19
| # Systeme | d’exploitation |     |     |     |     |
| --------- | -------------- | --- | --- | --- | --- |
20
21 .DS_Store
Thumbs.db
22
23
| # Dependances |     | Node.js |     |     |     |
| ------------- | --- | ------- | --- | --- | --- |
24
25 node_modules/
npm-debug.log
26
27
| 28 # Verifier    | quels | fichiers       | seront | ignores |     |
| ---------------- | ----- | -------------- | ------ | ------- | --- |
| git check-ignore |       | -v fichier.txt |        |         |     |
29
30
| # Forcer | l’ajout | d’un fichier | ignore |     |     |
| -------- | ------- | ------------ | ------ | --- | --- |
31
| 32 git add | -f fichier.log |              |           |            |            |
| ---------- | -------------- | ------------ | --------- | ---------- | ---------- |
|            |                | Listing 2.13 | – Exemple | de fichier | .gitignore |
13

| Chapitre       |     | 3   |          |           |     |     |      |
| -------------- | --- | --- | -------- | --------- | --- | --- | ---- |
| Intégration    |     |     | Continue |           |     |     | (CI) |
| 3.1 Définition |     |     | et       | Principes |     |     |      |
Intégration Continue (CI) : pratique consistant à intégrer fréquemment le code
des développeurs dans un dépôt partagé, chaque intégration étant vérifiée automati-
| quement        | par              | une série        | de tests    | et             | de       | vérifications. |                |
| -------------- | ---------------- | ---------------- | ----------- | -------------- | -------- | -------------- | -------------- |
| Les principes  | fondamentaux     |                  |             | de la          | CI sont  | :              |                |
| 1. Maintenir   |                  | un dépôt         | de          | code           | unique   | et             | partagé.       |
| 2. Automatiser |                  | la construction  |             |                | (build). |                |                |
| 3. Rendre      | la               | construction     |             | auto-testable. |          |                |                |
| 4. Intégrer    | quotidiennement. |                  |             |                |          |                |                |
| 5. Maintenir   |                  | un build         | rapide      | (moins         |          | de 10          | minutes).      |
| 6. Tester      | dans             | un environnement |             |                | clone    | de             | la production. |
| 7. Rendre      | les              | résultats        | accessibles |                | à        | tous.          |                |
| 8. Automatiser |                  | le déploiement.  |             |                |          |                |                |
| 3.2 Jenkins    |                  |                  |             |                |          |                |                |
| 3.2.1          | Présentation     |                  |             |                |          |                |                |
Jenkins est un serveur d’automatisation open-source écrit en Java. Il est le standard
de facto pour l’implémentation de pipelines CI/CD. Jenkins supporte des centaines de
plugins permettant l’intégration avec Git, Docker, Kubernetes, Slack, etc.
| 3.2.2       | Installation |      | de          | Jenkins |     |     |     |
| ----------- | ------------ | ---- | ----------- | ------- | --- | --- | --- |
| # Installer |              | Java | (prerequis) |         |     |     |     |
1
| sudo apt-get |     | update |     |     |     |     |     |
| ------------ | --- | ------ | --- | --- | --- | --- | --- |
2
| 3 sudo apt-get |     | install |     | -y  | openjdk-17-jdk |     |     |
| -------------- | --- | ------- | --- | --- | -------------- | --- | --- |
4
| # Ajouter |     | la cle | GPG | de  | Jenkins |     |     |
| --------- | --- | ------ | --- | --- | ------- | --- | --- |
5
curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.
6
| key | \   |     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- |
14

| Module |     | DevOps |     |     |     |     |     |     | S8-SIIA |
| ------ | --- | ------ | --- | --- | --- | --- | --- | --- | ------- |
| sudo tee /usr/share/keyrings/jenkins-keyring.asc > /dev/null
7
8
|     | # Ajouter |     | le  | depot | Jenkins |     |     |     |     |
| --- | --------- | --- | --- | ----- | ------- | --- | --- | --- | --- |
9
echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
10
| 11  | https://pkg.jenkins.io/debian-stable |     |     |                                      |     |     |     | binary/" | \           |
| --- | ------------------------------------ | --- | --- | ------------------------------------ | --- | --- | --- | -------- | ----------- |
|     | | sudo                               |     | tee | /etc/apt/sources.list.d/jenkins.list |     |     |     |          | > /dev/null |
12
13
|     | # Installer |     | Jenkins |     |     |     |     |     |     |
| --- | ----------- | --- | ------- | --- | --- | --- | --- | --- | --- |
14
| 15  | sudo | apt-get |     | update  |     |         |     |     |     |
| --- | ---- | ------- | --- | ------- | --- | ------- | --- | --- | --- |
|     | sudo | apt-get |     | install | -y  | jenkins |     |     |     |
16
17
| 18  | # Demarrer |           | et  | activer |         | Jenkins |     |     |     |
| --- | ---------- | --------- | --- | ------- | ------- | ------- | --- | --- | --- |
|     | sudo       | systemctl |     | start   | jenkins |         |     |     |     |
19
|     | sudo | systemctl |     | enable |     | jenkins |     |     |     |
| --- | ---- | --------- | --- | ------ | --- | ------- | --- | --- | --- |
20
21
| 22  | # Verifier |           | le  | statut |     |         |     |     |     |
| --- | ---------- | --------- | --- | ------ | --- | ------- | --- | --- | --- |
|     | sudo       | systemctl |     | status |     | jenkins |     |     |     |
23
24
| 25  | # Recuperer |     | le                                            | mot | de  | passe initial |     |     |     |
| --- | ----------- | --- | --------------------------------------------- | --- | --- | ------------- | --- | --- | --- |
|     | sudo        | cat | /var/lib/jenkins/secrets/initialAdminPassword |     |     |               |     |     |     |
26
|     |          |     |         | Listing | 3.1  | – Installation | de Jenkins | sur Ubuntu |     |
| --- | -------- | --- | ------- | ------- | ---- | -------------- | ---------- | ---------- | --- |
|     | # Lancer |     | Jenkins |         | dans | un conteneur   | Docker     |            |     |
1
|     | docker | run | -d  | \   |     |     |     |     |     |
| --- | ------ | --- | --- | --- | --- | --- | --- | --- | --- |
2
| 3   | --name |           | jenkins |     | \   |     |     |     |     |
| --- | ------ | --------- | ------- | --- | --- | --- | --- | --- | --- |
|     | -p     | 8080:8080 |         | \   |     |     |     |     |     |
4
|     | -p  | 50000:50000 |     |     | \   |     |     |     |     |
| --- | --- | ----------- | --- | --- | --- | --- | --- | --- | --- |
5
| 6   | -v  | jenkins_home:/var/jenkins_home |     |     |     |     | \   |     |     |
| --- | --- | ------------------------------ | --- | --- | --- | --- | --- | --- | --- |
jenkins/jenkins:lts-jdk17
7
8
|     | # Recuperer |     | le  | mot | de  | passe initial |     |     |     |
| --- | ----------- | --- | --- | --- | --- | ------------- | --- | --- | --- |
9
| 10  | docker | exec | jenkins |     | cat | /var/jenkins_home/secrets/ |     |     |     |
| --- | ------ | ---- | ------- | --- | --- | -------------------------- | --- | --- | --- |
initialAdminPassword
|       |               |         |     | Listing | 3.2     | – Installation | de Jenkins | via Docker |     |
| ----- | ------------- | ------- | --- | ------- | ------- | -------------- | ---------- | ---------- | --- |
| 3.2.3 |               | Gestion |     | de      | Jenkins | via CLI        |            |            |     |
|       | # Telecharger |         |     | le      | client  | CLI            |            |            |     |
1
| 2   | wget | http://localhost:8080/jnlpJars/jenkins-cli.jar |     |     |     |     |     |     |     |
| --- | ---- | ---------------------------------------------- | --- | --- | --- | --- | --- | --- | --- |
3
|     | # Se | connecter |     | au  | serveur | Jenkins |     |     |     |
| --- | ---- | --------- | --- | --- | ------- | ------- | --- | --- | --- |
4
|     | java | -jar | jenkins-cli.jar |     |     | \   |     |     |     |
| --- | ---- | ---- | --------------- | --- | --- | --- | --- | --- | --- |
5
| 6   | -s    | http://localhost:8080  |     |     |     | \   |     |     |     |
| --- | ----- | ---------------------- | --- | --- | --- | --- | --- | --- | --- |
|     | -auth | admin:mon-mot-de-passe |     |     |     |     | \   |     |     |
7
help
8
9
|     | # Lister |     | les | jobs |     |     |     |     |     |
| --- | -------- | --- | --- | ---- | --- | --- | --- | --- | --- |
10
|     | java | -jar | jenkins-cli.jar |     |     | \   |     |     |     |
| --- | ---- | ---- | --------------- | --- | --- | --- | --- | --- | --- |
11
|     | -s  | http://localhost:8080 |     |     |     | \   |     |     |     |
| --- | --- | --------------------- | --- | --- | --- | --- | --- | --- | --- |
12
| 13  | -auth | admin:token |     |     | \   |     |     |     |     |
| --- | ----- | ----------- | --- | --- | --- | --- | --- | --- | --- |
15

| Module | DevOps |     |     |     |     | S8-SIIA |
| ------ | ------ | --- | --- | --- | --- | ------- |
list-jobs
14
15
| # Declencher | un  | build |     |     |     |     |
| ------------ | --- | ----- | --- | --- | --- | --- |
16
| java | -jar jenkins-cli.jar |     |     | \   |     |     |
| ---- | -------------------- | --- | --- | --- | --- | --- |
17
| 18 -s | http://localhost:8080 |     |     | \   |     |     |
| ----- | --------------------- | --- | --- | --- | --- | --- |
| -auth | admin:token           |     | \   |     |     |     |
19
| build | mon-job |     |     |     |     |     |
| ----- | ------- | --- | --- | --- | --- | --- |
20
21
| 22 # Activer/desactiver |     |     | un  | job |     |     |
| ----------------------- | --- | --- | --- | --- | --- | --- |
java -jar jenkins-cli.jar -s http://localhost:8080 -auth admin:
23
| token | disable-job |     | mon-job |     |     |     |
| ----- | ----------- | --- | ------- | --- | --- | --- |
24 java -jar jenkins-cli.jar -s http://localhost:8080 -auth admin:
| token | enable-job |     | mon-job |     |     |     |
| ----- | ---------- | --- | ------- | --- | --- | --- |
25
| # Supprimer | un  | job |     |     |     |     |
| ----------- | --- | --- | --- | --- | --- | --- |
26
27 java -jar jenkins-cli.jar -s http://localhost:8080 -auth admin:
| token | delete-job |     | mon-job |     |     |     |
| ----- | ---------- | --- | ------- | --- | --- | --- |
28
| 29 # Installer | un  | plugin |     |     |     |     |
| -------------- | --- | ------ | --- | --- | --- | --- |
java -jar jenkins-cli.jar -s http://localhost:8080 -auth admin:
30
| token | install-plugin |     |     | git |     |     |
| ----- | -------------- | --- | --- | --- | --- | --- |
31
| # Recharger | la  | configuration |     |     |     |     |
| ----------- | --- | ------------- | --- | --- | --- | --- |
32
java -jar jenkins-cli.jar -s http://localhost:8080 -auth admin:
33
| token | reload-configuration |     |     |     |     |     |
| ----- | -------------------- | --- | --- | --- | --- | --- |
34
| # Redemarrer | Jenkins |     |     |     |     |     |
| ------------ | ------- | --- | --- | --- | --- | --- |
35
java -jar jenkins-cli.jar -s http://localhost:8080 -auth admin:
36
| token | restart     |            |         |     |               |     |
| ----- | ----------- | ---------- | ------- | --- | ------------- | --- |
|       |             |            | Listing |     | 3.3 – Jenkins | CLI |
| 3.2.4 | Jenkinsfile | – Pipeline |         |     | Déclaratif    |     |
Le Jenkinsfile est un fichier texte, placé à la racine du dépôt, qui décrit le pipeline de
| CI/CD      | au format Pipeline | as  | Code. |     |     |     |
| ---------- | ------------------ | --- | ----- | --- | --- | --- |
| 1 pipeline | {                  |     |       |     |     |     |
agent any
2
3
| 4   | environment | {   |      |             |     |     |
| --- | ----------- | --- | ---- | ----------- | --- | --- |
|     | MAVEN_HOME  | =   | tool | ’Maven-3.9’ |     |     |
5
|     | APP_VERSION |     | = ’1.0.0’ |     |     |     |
| --- | ----------- | --- | --------- | --- | --- | --- |
6
|     | DOCKER_IMAGE |     | = "monapp:${APP_VERSION}" |     |     |     |
| --- | ------------ | --- | ------------------------- | --- | --- | --- |
7
8 }
9
options {
10
| 11  | timeout(time: |     | 30, | unit: | ’MINUTES’) |     |
| --- | ------------- | --- | --- | ----- | ---------- | --- |
disableConcurrentBuilds()
12
buildDiscarder(logRotator(numToKeepStr: ’10’))
13
}
14
15
16

| Module DevOps |     |     |     |     |     |     |     |     |     | S8-SIIA |
| ------------- | --- | --- | --- | --- | --- | --- | --- | --- | --- | ------- |
triggers {
16
| 17  | pollSCM(’H/5 |     | * *       | * *’) |     | //  | Toutes |     | les  | 5 minutes  |
| --- | ------------ | --- | --------- | ----- | --- | --- | ------ | --- | ---- | ---------- |
|     | cron(’H      | 2   | * * 1-5’) |       |     | //  | Chaque |     | nuit | en semaine |
18
}
19
20
stages {
21
|     | stage(’Checkout’) |     |     | {   |     |     |     |     |     |     |
| --- | ----------------- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
22
|     | steps |     | {   |     |     |     |     |     |     |     |
| --- | ----- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
23
| 24  |     | git | branch: | ’main’,                                |     |     |     |     |     |     |
| --- | --- | --- | ------- | -------------------------------------- | --- | --- | --- | --- | --- | --- |
|     |     |     | url:    | ’https://github.com/utilisateur/depot. |     |     |     |     |     |     |
25
git’
| 26  | }   |     |     |     |     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
}
27
28
|     | stage(’Build’) |     | {   |     |     |     |     |     |     |     |
| --- | -------------- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
29
| 30  | steps |     | {                      |     |     |     |       |     |         |     |
| --- | ----- | --- | ---------------------- | --- | --- | --- | ----- | --- | ------- | --- |
|     |       | sh  | "${MAVEN_HOME}/bin/mvn |     |     |     | clean |     | package | -   |
31
DskipTests"
| 32  | }   |     |     |     |     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
}
33
34
|     | stage(’Tests |     | Unitaires’) |     | {   |     |     |     |     |     |
| --- | ------------ | --- | ----------- | --- | --- | --- | --- | --- | --- | --- |
35
|     | steps |     | {   |     |     |     |     |     |     |     |
| --- | ----- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
36
|     |     | sh  | "${MAVEN_HOME}/bin/mvn |     |     |     | test" |     |     |     |
| --- | --- | --- | ---------------------- | --- | --- | --- | ----- | --- | --- | --- |
37
}
38
| 39  | post | {      |     |     |     |     |     |     |     |     |
| --- | ---- | ------ | --- | --- | --- | --- | --- | --- | --- | --- |
|     |      | always | {   |     |     |     |     |     |     |     |
40
|     |     |     | junit | ’**/target/surefire-reports/*.xml’ |     |     |     |     |     |     |
| --- | --- | --- | ----- | ---------------------------------- | --- | --- | --- | --- | --- | --- |
41
| 42  |     | }   |     |     |     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
}
43
}
44
45
| 46  | stage(’Analyse |     | Qualite’) |     | {   |     |     |     |     |     |
| --- | -------------- | --- | --------- | --- | --- | --- | --- | --- | --- | --- |
|     | steps          |     | {         |     |     |     |     |     |     |     |
47
|     |     | withSonarQubeEnv(’SonarQube’) |     |     |     |     |     | {   |     |     |
| --- | --- | ----------------------------- | --- | --- | --- | --- | --- | --- | --- | --- |
48
| 49  |     |     | sh "${MAVEN_HOME}/bin/mvn |     |     |     |     | sonar:sonar" |     |     |
| --- | --- | --- | ------------------------- | --- | --- | --- | --- | ------------ | --- | --- |
}
50
}
51
}
52
53
|     | stage(’Quality |     | Gate’) | {   |     |     |     |     |     |     |
| --- | -------------- | --- | ------ | --- | --- | --- | --- | --- | --- | --- |
54
|     | steps |     | {   |     |     |     |     |     |     |     |
| --- | ----- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
55
| 56  |     | timeout(time: |                    | 5,  | unit: | ’MINUTES’)     |     |     | {   |      |
| --- | --- | ------------- | ------------------ | --- | ----- | -------------- | --- | --- | --- | ---- |
|     |     |               | waitForQualityGate |     |       | abortPipeline: |     |     |     | true |
57
}
58
}
59
| 60  | }   |     |     |     |     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
61
|     | stage(’Build |     | Docker’) | {   |     |     |     |     |     |     |
| --- | ------------ | --- | -------- | --- | --- | --- | --- | --- | --- | --- |
62
| 63  | steps |     | {       |       |     |                 |     |     |     |     |
| --- | ----- | --- | ------- | ----- | --- | --------------- | --- | --- | --- | --- |
|     |       | sh  | "docker | build | -t  | ${DOCKER_IMAGE} |     |     |     | ."  |
64
17

| Module DevOps |     |     |     |     |     |     |     |     |     |     |     | S8-SIIA |
| ------------- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | ------- |
}
65
| 66  | }   |     |     |     |     |     |     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
67
|     | stage(’Push |     |     | Image’) |     | {   |     |     |     |     |     |     |
| --- | ----------- | --- | --- | ------- | --- | --- | --- | --- | --- | --- | --- | --- |
68
| 69  |     | steps |     | {   |     |     |     |     |     |     |     |     |
| --- | --- | ----- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
withCredentials([usernamePassword(
70
|     |     |     |     | credentialsId: |     |     | ’docker-hub’, |     |     |     |     |     |
| --- | --- | --- | --- | -------------- | --- | --- | ------------- | --- | --- | --- | --- | --- |
71
|     |     |     |     | usernameVariable: |     |     |     | ’DOCKER_USER’, |     |     |     |     |
| --- | --- | --- | --- | ----------------- | --- | --- | --- | -------------- | --- | --- | --- | --- |
72
| 73  |     |     |     | passwordVariable: |     |     |     | ’DOCKER_PASS’ |     |     |     |     |
| --- | --- | --- | --- | ----------------- | --- | --- | --- | ------------- | --- | --- | --- | --- |
|     |     |     | )]) | {                 |     |     |     |               |     |     |     |     |
74
|     |     |     |     | sh  | """ |     |     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
75
| 76  |     |     |     |     | echo   | ${DOCKER_PASS} |     |                  | |   | docker | login -u | ${  |
| --- | --- | --- | --- | --- | ------ | -------------- | --- | ---------------- | --- | ------ | -------- | --- |
|     |     |     |     |     |        | DOCKER_USER}   |     | --password-stdin |     |        |          |     |
|     |     |     |     |     | docker | push           |     | ${DOCKER_IMAGE}  |     |        |          |     |
77
"""
78
| 79  |     |     | }   |     |     |     |     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
}
80
}
81
82
|     | stage(’Deploiement |     |     |     |     | Staging’) |     | {   |     |     |     |     |
| --- | ------------------ | --- | --- | --- | --- | --------- | --- | --- | --- | --- | --- | --- |
83
|     |     | when | {   |     |     |     |     |     |     |     |     |     |
| --- | --- | ---- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
84
|     |     |     | branch |     | ’develop’ |     |     |     |     |     |     |     |
| --- | --- | --- | ------ | --- | --------- | --- | --- | --- | --- | --- | --- | --- |
85
}
86
|     |     | steps |     | {   |     |     |     |     |     |     |     |     |
| --- | --- | ----- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
87
|     |     |     | sh  | "kubectl |     | apply | -f  | k8s/staging/" |     |     |     |     |
| --- | --- | --- | --- | -------- | --- | ----- | --- | ------------- | --- | --- | --- | --- |
88
| 89  |     | }   |     |     |     |     |     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
}
90
91
| 92  | stage(’Deploiement |      |     |     |     | Production’) |     | {   |     |     |     |     |
| --- | ------------------ | ---- | --- | --- | --- | ------------ | --- | --- | --- | --- | --- | --- |
|     |                    | when | {   |     |     |              |     |     |     |     |     |     |
93
|     |     |     | branch |     | ’main’ |     |     |     |     |     |     |     |
| --- | --- | --- | ------ | --- | ------ | --- | --- | --- | --- | --- | --- | --- |
94
}
95
| 96  |     | input |         | {   |           |     |     |            |     |     |     |     |
| --- | --- | ----- | ------- | --- | --------- | --- | --- | ---------- | --- | --- | --- | --- |
|     |     |       | message |     | "Deployer |     | en  | production |     | ?"  |     |     |
97
|     |     |     | ok  | "Deployer" |     |     |     |     |     |     |     |     |
| --- | --- | --- | --- | ---------- | --- | --- | --- | --- | --- | --- | --- | --- |
98
| 99  |     | }     |     |     |     |     |     |     |     |     |     |     |
| --- | --- | ----- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|     |     | steps |     | {   |     |     |     |     |     |     |     |     |
100
|     |     |     | sh  | "kubectl |     | apply | -f  | k8s/production/" |     |     |     |     |
| --- | --- | --- | --- | -------- | --- | ----- | --- | ---------------- | --- | --- | --- | --- |
101
}
102
| 103 | }   |     |     |     |     |     |     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
}
104
105
| 106 post | {       |     |     |     |     |     |     |     |     |     |     |     |
| -------- | ------- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|          | success |     | {   |     |     |     |     |     |     |     |     |     |
107
|     |     | slackSend |     |     | channel: | ’#devops’, |     |     |     |     |     |     |
| --- | --- | --------- | --- | --- | -------- | ---------- | --- | --- | --- | --- | --- | --- |
108
|     |     |     |     |     | message: | "Build |     | REUSSI | :   | ${env.JOB_NAME} |     | #   |
| --- | --- | --- | --- | --- | -------- | ------ | --- | ------ | --- | --------------- | --- | --- |
109
${env.BUILD_NUMBER}"
}
110
|     | failure |     | {   |     |     |     |     |     |     |     |     |     |
| --- | ------- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
111
| 112 |     | emailext |     | to:      | ’equipe@exemple.com’, |        |     |                   |     |     |         |     |
| --- | --- | -------- | --- | -------- | --------------------- | ------ | --- | ----------------- | --- | --- | ------- | --- |
|     |     |          |     | subject: |                       | "ECHEC |     | : ${env.JOB_NAME} |     |     | #${env. |     |
113
18

| Module | DevOps |     |     |     |     |     |     |     | S8-SIIA |
| ------ | ------ | --- | --- | --- | --- | --- | --- | --- | ------- |
BUILD_NUMBER}",
| 114 |     |     |     |     | body: | "Verifiez |     | les | logs : ${env.BUILD_URL} |
| --- | --- | --- | --- | --- | ----- | --------- | --- | --- | ----------------------- |
"
}
115
| 116 |     | always |     | {   |     |     |     |     |     |
| --- | --- | ------ | --- | --- | --- | --- | --- | --- | --- |
cleanWs()
117
}
118
}
119
120 }
|                 |     |           |     | Listing | 3.4 – | Structure   | d’un | Jenkinsfile | declaratif |
| --------------- | --- | --------- | --- | ------- | ----- | ----------- | ---- | ----------- | ---------- |
| 1 node(’linux’) |     |           |     | {       |       |             |      |             |            |
|                 | def | mavenHome |     | =       | tool  | ’Maven-3.9’ |      |             |            |
2
3
| 4   | stage(’Checkout’) |          |     |     | {   |     |     |     |     |
| --- | ----------------- | -------- | --- | --- | --- | --- | --- | --- | --- |
|     |                   | checkout |     | scm |     |     |     |     |     |
5
}
6
7
| 8   | stage(’Build’) |     |     |     | {   |     |     |     |     |
| --- | -------------- | --- | --- | --- | --- | --- | --- | --- | --- |
|     |                | try | {   |     |     |     |     |     |     |
9
|     |     |     | sh  | "${mavenHome}/bin/mvn |     |     |     | clean | package" |
| --- | --- | --- | --- | --------------------- | --- | --- | --- | ----- | -------- |
10
| 11  |     | }   | catch               | (Exception |     | e)  | {           |     |     |
| --- | --- | --- | ------------------- | ---------- | --- | --- | ----------- | --- | --- |
|     |     |     | currentBuild.result |            |     |     | = ’FAILURE’ |     |     |
12
|     |     |     | error | "Le | build |     | a echoue | : ${e.message}" |     |
| --- | --- | --- | ----- | --- | ----- | --- | -------- | --------------- | --- |
13
}
14
| 15  | }   |     |     |     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
16
|     | stage(’Deploiement’) |     |     |     |     | {   |     |     |     |
| --- | -------------------- | --- | --- | --- | --- | --- | --- | --- | --- |
17
| 18  |     | if  | (env.BRANCH_NAME |          |     |       | == ’main’) | {   |     |
| --- | --- | --- | ---------------- | -------- | --- | ----- | ---------- | --- | --- |
|     |     |     | sh               | ’kubectl |     | apply | -f k8s/’   |     |     |
19
}
20
}
21
22 }
|       |            |         |     | Listing |                   | 3.5 – Pipeline | Scripted | (Groovy) |     |
| ----- | ---------- | ------- | --- | ------- | ----------------- | -------------- | -------- | -------- | --- |
| 3.2.5 |            | Gestion |     | des     | Credentials       |                | Jenkins  |          |     |
| 1 //  | Credential |         |     | de type | Username/Password |                |          |          |     |
withCredentials([usernamePassword(
2
|     | credentialsId: |     |     |     | ’mon-credential-id’, |     |     |     |     |
| --- | -------------- | --- | --- | --- | -------------------- | --- | --- | --- | --- |
3
| 4   | usernameVariable: |     |     |     | ’USER’, |     |     |     |     |
| --- | ----------------- | --- | --- | --- | ------- | --- | --- | --- | --- |
|     | passwordVariable: |     |     |     | ’PASS’  |     |     |     |     |
5
| )]) | {   |     |     |     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
6
|     | sh  | "curl | -u  | ${USER}:${PASS} |     |     | https://api.exemple.com" |     |     |
| --- | --- | ----- | --- | --------------- | --- | --- | ------------------------ | --- | --- |
7
8 }
9
| //  | Credential |     |     | de type | Secret |     | Text |     |     |
| --- | ---------- | --- | --- | ------- | ------ | --- | ---- | --- | --- |
10
11 withCredentials([string(credentialsId: ’api-token’, variable: ’
|     | TOKEN’)]) |     | {   |     |     |     |     |     |     |
| --- | --------- | --- | --- | --- | --- | --- | --- | --- | --- |
19

| Module | DevOps   |     |                 |     |     |        |           |     |              | S8-SIIA |
| ------ | -------- | --- | --------------- | --- | --- | ------ | --------- | --- | ------------ | ------- |
|        | sh "curl | -H  | ’Authorization: |     |     | Bearer | ${TOKEN}’ |     | https://api. |         |
12
exemple.com"
}
13
14
| 15 // | Credential |     | de type | Fichier |     | Secret |     |     |     |     |
| ----- | ---------- | --- | ------- | ------- | --- | ------ | --- | --- | --- | --- |
withCredentials([file(credentialsId: ’kubeconfig’, variable: ’
16
|     | KUBECONFIG’)]) |     |                            | {   |     |     |     |     |       |     |
| --- | -------------- | --- | -------------------------- | --- | --- | --- | --- | --- | ----- | --- |
|     | sh "kubectl    |     | --kubeconfig=${KUBECONFIG} |     |     |     |     | get | pods" |     |
17
18 }
19
| //  | Credential |     | de type | SSH |     |     |     |     |     |     |
| --- | ---------- | --- | ------- | --- | --- | --- | --- | --- | --- | --- |
20
21 withCredentials([sshUserPrivateKey(
|     | credentialsId: |     |     | ’ssh-key’, |     |     |     |     |     |     |
| --- | -------------- | --- | --- | ---------- | --- | --- | --- | --- | --- | --- |
22
|     | keyFileVariable: |     |     | ’SSH_KEY’, |     |     |     |     |     |     |
| --- | ---------------- | --- | --- | ---------- | --- | --- | --- | --- | --- | --- |
23
|     | usernameVariable: |     |     | ’SSH_USER’ |     |     |     |     |     |     |
| --- | ----------------- | --- | --- | ---------- | --- | --- | --- | --- | --- | --- |
24
25 )]) {
|     | sh "ssh | -i  | ${SSH_KEY} |     | ${SSH_USER}@serveur.exemple.com |     |     |     |     | ’date’ |
| --- | ------- | --- | ---------- | --- | ------------------------------- | --- | --- | --- | --- | ------ |
26
"
27 }
|         |          | Listing |         | 3.6 – Utilisation |             | des | credentials | dans | Jenkins |     |
| ------- | -------- | ------- | ------- | ----------------- | ----------- | --- | ----------- | ---- | ------- | --- |
| 3.2.6   | GitHub   |         | Actions | –                 | Alternative |     | à Jenkins   |      |         |     |
| 1 name: | Pipeline |         | CI/CD   |                   |             |     |             |      |         |     |
2
on:
3
push:
4
| 5   | branches: |     | [main, | develop] |     |     |     |     |     |     |
| --- | --------- | --- | ------ | -------- | --- | --- | --- | --- | --- | --- |
pull_request:
6
|     | branches: |     | [main] |     |     |     |     |     |     |     |
| --- | --------- | --- | ------ | --- | --- | --- | --- | --- | --- | --- |
7
8
env:
9
|     | DOCKER_IMAGE: |     | monapp |     |     |     |     |     |     |     |
| --- | ------------- | --- | ------ | --- | --- | --- | --- | --- | --- | --- |
10
11
12 jobs:
build-and-test:
13
|     | runs-on: | ubuntu-latest |     |     |     |     |     |     |     |     |
| --- | -------- | ------------- | --- | --- | --- | --- | --- | --- | --- | --- |
14
15
steps:
16
|     | - name: |     | Checkout | du  | code |     |     |     |     |     |
| --- | ------- | --- | -------- | --- | ---- | --- | --- | --- | --- | --- |
17
|     | uses: |     | actions/checkout@v4 |     |     |     |     |     |     |     |
| --- | ----- | --- | ------------------- | --- | --- | --- | --- | --- | --- | --- |
18
19
|     | - name: |     | Configuration |     |     | de Java | 17  |     |     |     |
| --- | ------- | --- | ------------- | --- | --- | ------- | --- | --- | --- | --- |
20
|     | uses: |     | actions/setup-java@v4 |     |     |     |     |     |     |     |
| --- | ----- | --- | --------------------- | --- | --- | --- | --- | --- | --- | --- |
21
| 22  | with: |               |     |     |      |     |     |     |     |     |
| --- | ----- | ------------- | --- | --- | ---- | --- | --- | --- | --- | --- |
|     |       | java-version: |     |     | ’17’ |     |     |     |     |     |
23
|     |     | distribution: |     |     | ’temurin’ |     |     |     |     |     |
| --- | --- | ------------- | --- | --- | --------- | --- | --- | --- | --- | --- |
24
25
|     | - name: |     | Cache | Maven |     |     |     |     |     |     |
| --- | ------- | --- | ----- | ----- | --- | --- | --- | --- | --- | --- |
26
|     | uses: |     | actions/cache@v3 |     |     |     |     |     |     |     |
| --- | ----- | --- | ---------------- | --- | --- | --- | --- | --- | --- | --- |
27
20

| Module | DevOps |     |     |     |     |     |     | S8-SIIA |
| ------ | ------ | --- | --- | --- | --- | --- | --- | ------- |
with:
28
| 29  |     | path: | ~/.m2 |           |     |           |                         |     |
| --- | --- | ----- | ----- | --------- | --- | --------- | ----------------------- | --- |
|     |     | key:  | ${{   | runner.os |     | }}-m2-${{ | hashFiles(’**/pom.xml’) |     |
30
}}
31
|     | -   | name: | Build | et tests |     |     |     |     |
| --- | --- | ----- | ----- | -------- | --- | --- | --- | --- |
32
|     |     | run: | mvn | clean verify |     |     |     |     |
| --- | --- | ---- | --- | ------------ | --- | --- | --- | --- |
33
34
| 35  | -   | name: | Publication                |     | des | resultats | de  | tests |
| --- | --- | ----- | -------------------------- | --- | --- | --------- | --- | ----- |
|     |     | uses: | actions/upload-artifact@v4 |     |     |           |     |       |
36
with:
37
| 38  |     | name: | test-results             |     |     |     |     |     |
| --- | --- | ----- | ------------------------ | --- | --- | --- | --- | --- |
|     |     | path: | target/surefire-reports/ |     |     |     |     |     |
39
40
docker:
41
| 42  | needs:   | build-and-test |               |     |     |     |     |     |
| --- | -------- | -------------- | ------------- | --- | --- | --- | --- | --- |
|     | runs-on: |                | ubuntu-latest |     |     |     |     |     |
43
|     | if: | github.ref |     | == ’refs/heads/main’ |     |     |     |     |
| --- | --- | ---------- | --- | -------------------- | --- | --- | --- | --- |
44
45
steps:
46
|     | -   | uses: | actions/checkout@v4 |     |     |     |     |     |
| --- | --- | ----- | ------------------- | --- | --- | --- | --- | --- |
47
48
|     | -   | name: | Login | Docker | Hub |     |     |     |
| --- | --- | ----- | ----- | ------ | --- | --- | --- | --- |
49
|     |     | uses: | docker/login-action@v3 |     |     |     |     |     |
| --- | --- | ----- | ---------------------- | --- | --- | --- | --- | --- |
50
with:
51
| 52  |     | username: |     | ${{ | secrets.DOCKER_USERNAME |     |     | }}  |
| --- | --- | --------- | --- | --- | ----------------------- | --- | --- | --- |
|     |     | password: |     | ${{ | secrets.DOCKER_PASSWORD |     |     | }}  |
53
54
| 55  | -   | name: | Build                       | et Push |     | de l’image |     |     |
| --- | --- | ----- | --------------------------- | ------- | --- | ---------- | --- | --- |
|     |     | uses: | docker/build-push-action@v5 |         |     |            |     |     |
56
with:
57
|     |     | push: | true |     |     |     |     |     |
| --- | --- | ----- | ---- | --- | --- | --- | --- | --- |
58
| 59  |     | tags: | ${{          | secrets.DOCKER_USERNAME |           |     |     | }}/${{ env. |
| --- | --- | ----- | ------------ | ----------------------- | --------- | --- | --- | ----------- |
|     |     |       | DOCKER_IMAGE |                         | }}:latest |     |     |             |
Listing 3.7 – Workflow GitHub Actions (.github/workflows/ci.yml)
21

| Chapitre        | 4   |             |         |      |
| --------------- | --- | ----------- | ------- | ---- |
| Livraison       | et  | Déploiement | Continu | (CD) |
| 4.1 Définitions |     |             |         |      |
Livraison Continue (Continuous Delivery) : extension de la CI qui garantit que
le code peut être déployé en production à tout moment, après validation manuelle.
Déploiement Continu (Continuous Deployment) : extension de la livraison
continue où chaque modification validée par les tests est automatiquement déployée
| en production,   | sans intervention | humaine.       |     |     |
| ---------------- | ----------------- | -------------- | --- | --- |
| 4.2 Stratégies   |                   | de Déploiement |     |     |
| 4.2.1 Blue-Green |                   | Deployment     |     |     |
Deux environnements identiques (Blue = actuel, Green = nouveau) coexistent. Le trafic
est basculé vers Green une fois les tests validés. En cas de problème, le retour arrière est
immédiat.
| 4.2.2 Canary | Deployment |     |     |     |
| ------------ | ---------- | --- | --- | --- |
La nouvelle version est déployée progressivement : d’abord pour 5% des utilisateurs, puis
25%, puis 100%. Permet de détecter les régressions avant un impact total.
| 4.2.3 Rolling | Update |     |     |     |
| ------------- | ------ | --- | --- | --- |
Les instances de l’application sont mises à jour progressivement, une par une ou par
| groupes, sans | interruption | de service. |     |     |
| ------------- | ------------ | ----------- | --- | --- |
| 4.2.4 Feature | Flags        |             |     |     |
Les nouvelles fonctionnalités sont déployées dans le code mais masquées par des indica-
teurs configurables, permettant une activation progressive sans nouveau déploiement.
22

| Chapitre         |              |     | 5   |     |     |      |     |        |     |     |
| ---------------- | ------------ | --- | --- | --- | --- | ---- | --- | ------ | --- | --- |
| Conteneurisation |              |     |     |     |     | avec |     | Docker |     |     |
| 5.1              | Introduction |     |     |     |     |      |     |        |     |     |
Conteneur : unité d’exécution légère et isolée qui regroupe une application et toutes
ses dépendances (bibliothèques, configuration, code) dans un environnement standar-
|     | disé et portable. |     |     |     |     |     |     |     |     |     |
| --- | ----------------- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
Docker est la plateforme de conteneurisation la plus utilisée. Elle repose sur les fonction-
nalités du noyau Linux : namespaces (isolation) et cgroups (limitation des ressources).
| 5.2 | Installation |     |               | de  | Docker |          |     |     |     |     |
| --- | ------------ | --- | ------------- | --- | ------ | -------- | --- | --- | --- | --- |
|     | # Supprimer  |     | les anciennes |     |        | versions |     |     |     |     |
1
2 sudo apt-get remove -y docker docker-engine docker.io containerd
runc
3
| 4   | # Installer  |     | les dependances |     |     |     |     |     |     |     |
| --- | ------------ | --- | --------------- | --- | --- | --- | --- | --- | --- | --- |
|     | sudo apt-get |     | update          |     |     |     |     |     |     |     |
5
|     | sudo apt-get |     | install |     | -y \ |     |     |     |     |     |
| --- | ------------ | --- | ------- | --- | ---- | --- | --- | --- | --- | --- |
6
|     | ca-certificates |     |     | \   |     |     |     |     |     |     |
| --- | --------------- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
7
| 8   | curl  | \   |     |     |     |     |     |     |     |     |
| --- | ----- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|     | gnupg | \   |     |     |     |     |     |     |     |     |
9
lsb-release
10
11
|     | # Ajouter | la  | cle | GPG | officielle |     | de  | Docker |     |     |
| --- | --------- | --- | --- | --- | ---------- | --- | --- | ------ | --- | --- |
12
|     | sudo mkdir |     | -p /etc/apt/keyrings |     |     |     |     |     |     |     |
| --- | ---------- | --- | -------------------- | --- | --- | --- | --- | --- | --- | --- |
13
|     | curl -fsSL |     | https://download.docker.com/linux/ubuntu/gpg |     |     |     |     |     |     | \   |
| --- | ---------- | --- | -------------------------------------------- | --- | --- | --- | --- | --- | --- | --- |
14
| 15  | | sudo | gpg | --dearmor |     | -o  | /etc/apt/keyrings/docker.gpg |     |     |     |     |
| --- | ------ | --- | --------- | --- | --- | ---------------------------- | --- | --- | --- | --- |
16
|     | # Ajouter | le  | depot | Docker |     |     |     |     |     |     |
| --- | --------- | --- | ----- | ------ | --- | --- | --- | --- | --- | --- |
17
| 18  | echo \ |              |     |                       |     |     |     |     |     |     |
| --- | ------ | ------------ | --- | --------------------- | --- | --- | --- | --- | --- | --- |
|     | "deb   | [arch=$(dpkg |     | --print-architecture) |     |     |     |     | \   |     |
19
|     | signed-by=/etc/apt/keyrings/docker.gpg] |     |     |     |     |     |     |     | \   |     |
| --- | --------------------------------------- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
20
|     | https://download.docker.com/linux/ubuntu |     |     |     |     |     |     |     | \   |     |
| --- | ---------------------------------------- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
21
|     | $(lsb_release |     | -cs) |     | stable" | \   |     |     |     |     |
| --- | ------------- | --- | ---- | --- | ------- | --- | --- | --- | --- | --- |
22
23

| Module |        | DevOps |                                         |     |     |     |     | S8-SIIA     |
| ------ | ------ | ------ | --------------------------------------- | --- | --- | --- | --- | ----------- |
|        | | sudo |        | tee /etc/apt/sources.list.d/docker.list |     |     |     |     | > /dev/null |
23
24
|     | # Installer |     | Docker | Engine |     |     |     |     |
| --- | ----------- | --- | ------ | ------ | --- | --- | --- | --- |
25
|     | sudo | apt-get | update |     |     |     |     |     |
| --- | ---- | ------- | ------ | --- | --- | --- | --- | --- |
26
| 27  | sudo      | apt-get | install |     | -y \ |     |     |     |
| --- | --------- | ------- | ------- | --- | ---- | --- | --- | --- |
|     | docker-ce |         | \       |     |      |     |     |     |
28
|     | docker-ce-cli |     |     | \   |     |     |     |     |
| --- | ------------- | --- | --- | --- | --- | --- | --- | --- |
29
|     | containerd.io |     |     | \   |     |     |     |     |
| --- | ------------- | --- | --- | --- | --- | --- | --- | --- |
30
| 31  | docker-buildx-plugin |     |     |     | \   |     |     |     |
| --- | -------------------- | --- | --- | --- | --- | --- | --- | --- |
docker-compose-plugin
32
33
| 34  | # Demarrer |           | Docker |     |        |     |     |     |
| --- | ---------- | --------- | ------ | --- | ------ | --- | --- | --- |
|     | sudo       | systemctl | start  |     | docker |     |     |     |
35
|     | sudo | systemctl | enable |     | docker |     |     |     |
| --- | ---- | --------- | ------ | --- | ------ | --- | --- | --- |
36
37
| 38  | # Verifier |         | l’installation |     |     |     |     |     |
| --- | ---------- | ------- | -------------- | --- | --- | --- | --- | --- |
|     | docker     | version |                |     |     |     |     |     |
39
|     | docker | info |     |     |     |     |     |     |
| --- | ------ | ---- | --- | --- | --- | --- | --- | --- |
40
41
|     | # Ajouter |     | l’utilisateur |     | au groupe | docker | (eviter | sudo) |
| --- | --------- | --- | ------------- | --- | --------- | ------ | ------- | ----- |
42
|     | sudo | usermod | -aG docker |     | $USER |     |     |     |
| --- | ---- | ------- | ---------- | --- | ----- | --- | --- | --- |
43
|     | newgrp | docker |     |     |     |     |     |     |
| --- | ------ | ------ | --- | --- | --- | --- | --- | --- |
44
|     |              |         | Listing   | 5.1    | – Installation | de Docker | sur Ubuntu |     |
| --- | ------------ | ------- | --------- | ------ | -------------- | --------- | ---------- | --- |
| 5.3 |              | Gestion | des       | Images |                |           |            |     |
|     | # Rechercher |         | une image |        | sur Docker     | Hub       |            |     |
1
|     | docker | search | ubuntu |     |     |     |     |     |
| --- | ------ | ------ | ------ | --- | --- | --- | --- | --- |
2
3
|     | # Telecharger |     | une | image |     |     |     |     |
| --- | ------------- | --- | --- | ----- | --- | --- | --- | --- |
4
|     | docker | pull | ubuntu:22.04 |     |     |     |     |     |
| --- | ------ | ---- | ------------ | --- | --- | --- | --- | --- |
5
| 6   | docker | pull | nginx:latest     |     |     |     |     |     |
| --- | ------ | ---- | ---------------- | --- | --- | --- | --- | --- |
|     | docker | pull | python:3.11-slim |     |     |     |     |     |
7
8
|     | # Lister |     | les images | locales |     |     |     |     |
| --- | -------- | --- | ---------- | ------- | --- | --- | --- | --- |
9
| 10  | docker | images |     |     |     |     |     |     |
| --- | ------ | ------ | --- | --- | --- | --- | --- | --- |
|     | docker | image  | ls  |     |     |     |     |     |
11
12
| 13  | # Lister |       | toutes les | images | (inclus | les | intermediaires) |     |
| --- | -------- | ----- | ---------- | ------ | ------- | --- | --------------- | --- |
|     | docker   | image | ls -a      |        |         |     |                 |     |
14
15
|     | # Afficher |     | les details |     | d’une image |     |     |     |
| --- | ---------- | --- | ----------- | --- | ----------- | --- | --- | --- |
16
| 17  | docker | image | inspect |     | ubuntu:22.04 |     |     |     |
| --- | ------ | ----- | ------- | --- | ------------ | --- | --- | --- |
18
|     | # Afficher |     | l’historique |     | d’une image |     |     |     |
| --- | ---------- | --- | ------------ | --- | ----------- | --- | --- | --- |
19
| 20  | docker | image | history |     | ubuntu:22.04 |     |     |     |
| --- | ------ | ----- | ------- | --- | ------------ | --- | --- | --- |
21
|     | # Supprimer |     | une image |     |     |     |     |     |
| --- | ----------- | --- | --------- | --- | --- | --- | --- | --- |
22
|     | docker | image | rm ubuntu:22.04 |     |     |     |     |     |
| --- | ------ | ----- | --------------- | --- | --- | --- | --- | --- |
23
| 24  | docker | rmi | ubuntu:22.04 |     |     |     |     |     |
| --- | ------ | --- | ------------ | --- | --- | --- | --- | --- |
24

| Module | DevOps |     |     |     |     |     |     |     |     | S8-SIIA |
| ------ | ------ | --- | --- | --- | --- | --- | --- | --- | --- | ------- |
25
| 26 # Supprimer |       | les   | images |     | non utilisees |     |     |     |     |     |
| -------------- | ----- | ----- | ------ | --- | ------------- | --- | --- | --- | --- | --- |
| docker         | image | prune |        |     |               |     |     |     |     |     |
27
28
29 # Supprimer toutes les images non utilisees (y compris taggees)
| docker | image | prune |     | -a  |     |     |     |     |     |     |
| ------ | ----- | ----- | --- | --- | --- | --- | --- | --- | --- | --- |
30
31
| # Tagger |     | une image |     |     |     |     |     |     |     |     |
| -------- | --- | --------- | --- | --- | --- | --- | --- | --- | --- | --- |
32
33 docker tag monapp:latest mon-registry.exemple.com/monapp:v1.0.0
34
| # Pousser |     | une image |     | vers | un  | registre |     |     |     |     |
| --------- | --- | --------- | --- | ---- | --- | -------- | --- | --- | --- | --- |
35
| 36 docker | push | mon-registry.exemple.com/monapp:v1.0.0 |     |     |     |     |     |     |     |     |
| --------- | ---- | -------------------------------------- | --- | --- | --- | --- | --- | --- | --- | --- |
37
| # Sauvegarder |     | une | image |     | dans | un  | fichier |     | tar |     |
| ------------- | --- | --- | ----- | --- | ---- | --- | ------- | --- | --- | --- |
38
| docker | save | -o  | monapp.tar |     | monapp:latest |     |     |     |     |     |
| ------ | ---- | --- | ---------- | --- | ------------- | --- | --- | --- | --- | --- |
39
40
| # Charger |     | une image |     | depuis | un  | fichier |     | tar |     |     |
| --------- | --- | --------- | --- | ------ | --- | ------- | --- | --- | --- | --- |
41
| docker | load | -i  | monapp.tar |     |     |     |     |     |     |     |
| ------ | ---- | --- | ---------- | --- | --- | --- | --- | --- | --- | --- |
42
43
| # Exporter |     | le systeme |     | de  | fichiers |     | d’un | conteneur |     |     |
| ---------- | --- | ---------- | --- | --- | -------- | --- | ---- | --------- | --- | --- |
44
| docker | export | mon-conteneur |     |     |     | -o  | conteneur.tar |     |     |     |
| ------ | ------ | ------------- | --- | --- | --- | --- | ------------- | --- | --- | --- |
45
46
| # Importer |     | comme | image |     |     |     |     |     |     |     |
| ---------- | --- | ----- | ----- | --- | --- | --- | --- | --- | --- | --- |
47
| docker | import | conteneur.tar |     |     |     | mon-image:importee |     |     |     |     |
| ------ | ------ | ------------- | --- | --- | --- | ------------------ | --- | --- | --- | --- |
48
|           |         | Listing      | 5.2 | – Commandes |           | de  | gestion | des | images | Docker |
| --------- | ------- | ------------ | --- | ----------- | --------- | --- | ------- | --- | ------ | ------ |
| 5.4       | Gestion |              | des | Conteneurs  |           |     |         |     |        |        |
| 1 # Creer | et      | demarrer     |     | un          | conteneur |     |         |     |        |        |
| docker    | run     | ubuntu:22.04 |     |             |           |     |         |     |        |        |
2
3
| 4 # Demarrer |     | un conteneur |              |     | en mode |           | interactif |     |     |     |
| ------------ | --- | ------------ | ------------ | --- | ------- | --------- | ---------- | --- | --- | --- |
| docker       | run | -it          | ubuntu:22.04 |     |         | /bin/bash |            |     |     |     |
5
6
| # Demarrer |     | en arriere-plan |     |     | (detached) |     |     |     |     |     |
| ---------- | --- | --------------- | --- | --- | ---------- | --- | --- | --- | --- | --- |
7
| 8 docker | run | -d --name |     | mon-nginx |     |     | nginx:latest |     |     |     |
| -------- | --- | --------- | --- | --------- | --- | --- | ------------ | --- | --- | --- |
9
| # Demarrer |     | avec | mappage |     | de ports |     |     |     |     |     |
| ---------- | --- | ---- | ------- | --- | -------- | --- | --- | --- | --- | --- |
10
| 11 docker | run | -d -p | 8080:80 |     | --name |     | mon-nginx |     | nginx:latest |     |
| --------- | --- | ----- | ------- | --- | ------ | --- | --------- | --- | ------------ | --- |
12
| # Demarrer |     | avec | variables |     | d’environnement |     |     |     |     |     |
| ---------- | --- | ---- | --------- | --- | --------------- | --- | --- | --- | --- | --- |
13
| docker | run | -d \ |     |     |     |     |     |     |     |     |
| ------ | --- | ---- | --- | --- | --- | --- | --- | --- | --- | --- |
14
| 15 -e | MYSQL_ROOT_PASSWORD=secret |     |     |     |     |     | \   |     |     |     |
| ----- | -------------------------- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| -e    | MYSQL_DATABASE=mabase      |     |     |     | \   |     |     |     |     |     |
16
| --name |     | mon-mysql |     | \   |     |     |     |     |     |     |
| ------ | --- | --------- | --- | --- | --- | --- | --- | --- | --- | --- |
17
18 mysql:8.0
19
| # Demarrer |     | avec | volume |     | monte |     |     |     |     |     |
| ---------- | --- | ---- | ------ | --- | ----- | --- | --- | --- | --- | --- |
20
| docker | run | -d \ |     |     |     |     |     |     |     |     |
| ------ | --- | ---- | --- | --- | --- | --- | --- | --- | --- | --- |
21
| 22 -v | /chemin/hote:/chemin/conteneur |     |     |     |     |     |     | \   |     |     |
| ----- | ------------------------------ | --- | --- | --- | --- | --- | --- | --- | --- | --- |
25

Module DevOps S8-SIIA
--name mon-app \
23
monapp:latest
24
25
# Demarrer avec limites de ressources
26
docker run -d \
27
--memory="512m" \
28
--cpus="1.5" \
29
--name mon-app \
30
monapp:latest
31
32
# Demarrer avec politique de redemarrage
33
docker run -d \
34
--restart unless-stopped \
35
--name mon-app \
36
monapp:latest
37
38
# Lister les conteneurs en cours d’execution
39
docker ps
40
docker container ls
41
42
# Lister tous les conteneurs (arrets inclus)
43
docker ps -a
44
45
# Afficher les statistiques en temps reel
46
docker stats
47
48
# Afficher les statistiques d’un seul conteneur
49
docker stats mon-nginx
50
51
# Inspecter un conteneur
52
docker inspect mon-nginx
53
54
# Afficher les logs d’un conteneur
55
docker logs mon-nginx
56
57
# Suivre les logs en temps reel
58
docker logs -f mon-nginx
59
60
# Afficher les 100 dernieres lignes
61
docker logs --tail 100 mon-nginx
62
63
# Executer une commande dans un conteneur en cours d’execution
64
docker exec -it mon-nginx /bin/bash
65
docker exec mon-nginx ls /var/www/html
66
67
# Copier des fichiers entre l’hote et un conteneur
68
docker cp fichier.txt mon-nginx:/var/www/html/
69
docker cp mon-nginx:/var/log/nginx/access.log .
70
71
# Arreter un conteneur (SIGTERM, puis SIGKILL apres 10s)
72
docker stop mon-nginx
73
26

| Module | DevOps |     |     |     |     |     |     |     | S8-SIIA |
| ------ | ------ | --- | --- | --- | --- | --- | --- | --- | ------- |
74
| 75 # Forcer |      | l’arret   | immediatement |     |     | (SIGKILL) |     |     |     |
| ----------- | ---- | --------- | ------------- | --- | --- | --------- | --- | --- | --- |
| docker      | kill | mon-nginx |               |     |     |           |     |     |     |
76
77
| 78 # Demarrer |       | un  | conteneur |     | arrete |     |     |     |     |
| ------------- | ----- | --- | --------- | --- | ------ | --- | --- | --- | --- |
| docker        | start |     | mon-nginx |     |        |     |     |     |     |
79
80
| # Redemarrer |     |     | un conteneur |     |     |     |     |     |     |
| ------------ | --- | --- | ------------ | --- | --- | --- | --- | --- | --- |
81
| 82 docker | restart |     | mon-nginx |     |     |     |     |     |     |
| --------- | ------- | --- | --------- | --- | --- | --- | --- | --- | --- |
83
| # Mettre |     | en pause | /   | reprendre |     |     |     |     |     |
| -------- | --- | -------- | --- | --------- | --- | --- | --- | --- | --- |
84
| 85 docker | pause   |     | mon-nginx |     |     |     |     |     |     |
| --------- | ------- | --- | --------- | --- | --- | --- | --- | --- | --- |
| docker    | unpause |     | mon-nginx |     |     |     |     |     |     |
86
87
| # Supprimer |     | un  | conteneur |     | (il | doit etre | arrete) |     |     |
| ----------- | --- | --- | --------- | --- | --- | --------- | ------- | --- | --- |
88
| 89 docker | rm  | mon-nginx |     |     |     |     |     |     |     |
| --------- | --- | --------- | --- | --- | --- | --- | --- | --- | --- |
90
| # Supprimer |     | un  | conteneur |     | en  | cours d’execution |     |     |     |
| ----------- | --- | --- | --------- | --- | --- | ----------------- | --- | --- | --- |
91
| 92 docker | rm  | -f  | mon-nginx |     |     |     |     |     |     |
| --------- | --- | --- | --------- | --- | --- | --- | --- | --- | --- |
93
| # Supprimer |     | tous | les | conteneurs |     | arretes |     |     |     |
| ----------- | --- | ---- | --- | ---------- | --- | ------- | --- | --- | --- |
94
| docker | container |     | prune |     |     |     |     |     |     |
| ------ | --------- | --- | ----- | --- | --- | --- | --- | --- | --- |
95
96
| # Renommer |     | un  | conteneur |     |     |     |     |     |     |
| ---------- | --- | --- | --------- | --- | --- | --- | --- | --- | --- |
97
| docker | rename |     | mon-nginx |     | nouveau-nom |     |     |     |     |
| ------ | ------ | --- | --------- | --- | ----------- | --- | --- | --- | --- |
98
99
| # Afficher |     | les | ports | exposees |     |     |     |     |     |
| ---------- | --- | --- | ----- | -------- | --- | --- | --- | --- | --- |
100
| docker | port | mon-nginx |     |     |     |     |     |     |     |
| ------ | ---- | --------- | --- | --- | --- | --- | --- | --- | --- |
101
102
| # Afficher |     | les | processus |     | dans | un conteneur |     |     |     |
| ---------- | --- | --- | --------- | --- | ---- | ------------ | --- | --- | --- |
103
| docker | top | mon-nginx |     |     |     |     |     |     |     |
| ------ | --- | --------- | --- | --- | --- | --- | --- | --- | --- |
104
105
| 106 # Attendre |      | qu’un     | conteneur |     | s’arrete |     |     |     |     |
| -------------- | ---- | --------- | --------- | --- | -------- | --- | --- | --- | --- |
| docker         | wait | mon-nginx |           |     |          |     |     |     |     |
107
|          |              |            | Listing | 5.3 – | Commandes | de gestion | des conteneurs |     |     |
| -------- | ------------ | ---------- | ------- | ----- | --------- | ---------- | -------------- | --- | --- |
| 5.5      | Le           | Dockerfile |         |       |           |            |                |     |     |
| 1 # FROM | :            | image      | de base |       |           |            |                |     |     |
| FROM     | ubuntu:22.04 |            |         |       |           |            |                |     |     |
2
| FROM | python:3.11-slim |     |     | AS  | base |     |     |     |     |
| ---- | ---------------- | --- | --- | --- | ---- | --- | --- | --- | --- |
3
4
| 5 # LABEL | :                                 | metadonnees |     | de  | l’image |     |     |     |     |
| --------- | --------------------------------- | ----------- | --- | --- | ------- | --- | --- | --- | --- |
| LABEL     | maintainer="aattouri@exemple.com" |             |     |     |         |     |     |     |     |
6
| LABEL | version="1.0" |     |     |     |     |     |     |     |     |
| ----- | ------------- | --- | --- | --- | --- | --- | --- | --- | --- |
7
| 8 LABEL | description="Application |     |     |     |     | DevOps" |     |     |     |
| ------- | ------------------------ | --- | --- | --- | --- | ------- | --- | --- | --- |
9
| # ARG | :   | argument | de  | build | (disponible |     | uniquement | pendant | le  |
| ----- | --- | -------- | --- | ----- | ----------- | --- | ---------- | ------- | --- |
10
build)
| 11 ARG | APP_VERSION=1.0.0 |     |     |     |     |     |     |     |     |
| ------ | ----------------- | --- | --- | --- | --- | --- | --- | --- | --- |
27

Module DevOps S8-SIIA
ARG BUILD_DATE
12
13
# ENV : variable d’environnement (disponible a l’execution)
14
ENV APP_HOME=/app
15
ENV APP_VERSION=${APP_VERSION}
16
ENV PYTHONDONTWRITEBYTECODE=1
17
ENV PYTHONUNBUFFERED=1
18
19
# WORKDIR : repertoire de travail
20
WORKDIR /app
21
22
# RUN : executer une commande pendant le build
23
RUN apt-get update \
24
&& apt-get install -y --no-install-recommends \
25
curl \
26
wget \
27
&& rm -rf /var/lib/apt/lists/*
28
29
# COPY : copier des fichiers de l’hote vers l’image
30
COPY requirements.txt .
31
COPY src/ ./src/
32
33
# ADD : comme COPY mais supporte URL et .tar.gz (deconseille
34
sauf besoin specifique)
ADD https://exemple.com/fichier.tar.gz /tmp/
35
36
# RUN pour installer les dependances Python
37
RUN pip install --no-cache-dir -r requirements.txt
38
39
# USER : changer l’utilisateur courant
40
RUN adduser --system --group appuser
41
USER appuser
42
43
# EXPOSE : documenter le port expose (ne publie pas)
44
EXPOSE 8080
45
46
# VOLUME : creer un point de montage
47
VOLUME ["/app/data", "/app/logs"]
48
49
# HEALTHCHECK : verifier la sante du conteneur
50
HEALTHCHECK --interval=30s --timeout=10s --start-period=5s --
51
retries=3 \
CMD curl -f http://localhost:8080/health || exit 1
52
53
# ENTRYPOINT : commande principale (non surchargeable sans --
54
entrypoint)
ENTRYPOINT ["python", "-m", "gunicorn"]
55
56
# CMD : arguments par defaut de ENTRYPOINT (surchargeable)
57
CMD ["--bind", "0.0.0.0:8080", "app:application"]
58
Listing 5.4 – Instruction du Dockerfile
28

Module DevOps S8-SIIA
# Stage 1 : Build
1
FROM maven:3.9-openjdk-17 AS builder
2
WORKDIR /build
3
COPY pom.xml .
4
COPY src ./src
5
RUN mvn clean package -DskipTests
6
7
# Stage 2 : Production (image finale legere)
8
FROM openjdk:17-jre-slim AS production
9
WORKDIR /app
10
11
# Creer un utilisateur non-root
12
RUN addgroup --system --gid 1001 appgroup \
13
&& adduser --system --uid 1001 --gid 1001 appuser
14
15
# Copier uniquement le JAR depuis le stage de build
16
COPY --from=builder /build/target/monapp.jar app.jar
17
18
USER appuser
19
EXPOSE 8080
20
21
HEALTHCHECK --interval=30s --timeout=5s \
22
CMD wget -qO- http://localhost:8080/actuator/health || exit 1
23
24
ENTRYPOINT ["java", "-jar", "/app/app.jar"]
25
Listing 5.5 – Multi-stage Build (bonne pratique)
5.5.1 Construction d’Images
# Construire une image depuis le Dockerfile courant
1
docker build -t monapp:latest .
2
3
# Specifier un Dockerfile alternatif
4
docker build -f Dockerfile.prod -t monapp:prod .
5
6
# Passer des arguments de build
7
docker build \
8
--build-arg APP_VERSION=2.0.0 \
9
--build-arg BUILD_DATE=$(date -u +"%Y-%m-%dT%H:%M:%SZ") \
10
-t monapp:2.0.0 .
11
12
# Construire sans cache
13
docker build --no-cache -t monapp:latest .
14
15
# Specifier la plateforme cible
16
docker build --platform linux/amd64 -t monapp:latest .
17
18
# Build multi-plateforme avec BuildKit
19
docker buildx build \
20
--platform linux/amd64,linux/arm64 \
21
29

Module DevOps S8-SIIA
-t monapp:latest \
22
--push .
23
24
# Afficher les etapes de build
25
docker build --progress=plain -t monapp:latest .
26
27
# Cibler un stage specifique (multi-stage)
28
docker build --target builder -t monapp:build .
29
Listing 5.6 – Commandes de build Docker
5.6 Réseaux Docker
# Lister les reseaux
1
docker network ls
2
3
# Inspecter un reseau
4
docker network inspect bridge
5
6
# Creer un reseau personnalise
7
docker network create mon-reseau
8
9
# Creer un reseau avec sous-reseau specifique
10
docker network create \
11
--driver bridge \
12
--subnet 192.168.10.0/24 \
13
--gateway 192.168.10.1 \
14
mon-reseau-custom
15
16
# Connecter un conteneur a un reseau
17
docker network connect mon-reseau mon-conteneur
18
19
# Deconnecter un conteneur d’un reseau
20
docker network disconnect mon-reseau mon-conteneur
21
22
# Supprimer un reseau
23
docker network rm mon-reseau
24
25
# Supprimer tous les reseaux non utilises
26
docker network prune
27
28
# Demarrer un conteneur sur un reseau specifique
29
docker run -d \
30
--network mon-reseau \
31
--name mon-app \
32
monapp:latest
33
Listing 5.7 – Gestion des reseaux Docker
30

| Module |          | DevOps  |         |        |     |     |     | S8-SIIA |
| ------ | -------- | ------- | ------- | ------ | --- | --- | --- | ------- |
| 5.7    |          | Volumes |         | Docker |     |     |     |         |
|        | # Lister | les     | volumes |        |     |     |     |         |
1
|     | docker | volume |     | ls  |     |     |     |     |
| --- | ------ | ------ | --- | --- | --- | --- | --- | --- |
2
3
| 4   | # Creer | un     | volume |        | nomme       |     |     |     |
| --- | ------- | ------ | ------ | ------ | ----------- | --- | --- | --- |
|     | docker  | volume |        | create | mes-donnees |     |     |     |
5
6
| 7   | # Inspecter |        | un  | volume  |     |             |     |     |
| --- | ----------- | ------ | --- | ------- | --- | ----------- | --- | --- |
|     | docker      | volume |     | inspect |     | mes-donnees |     |     |
8
9
|     | # Supprimer |     | un  | volume |     |     |     |     |
| --- | ----------- | --- | --- | ------ | --- | --- | --- | --- |
10
| 11  | docker | volume |     | rm mes-donnees |     |     |     |     |
| --- | ------ | ------ | --- | -------------- | --- | --- | --- | --- |
12
|     | # Supprimer |     | les | volumes |     | non | utilises |     |
| --- | ----------- | --- | --- | ------- | --- | --- | -------- | --- |
13
| 14  | docker | volume |     | prune |     |     |     |     |
| --- | ------ | ------ | --- | ----- | --- | --- | --- | --- |
15
|     | # Monter | un  | volume |     | nomme |     |     |     |
| --- | -------- | --- | ------ | --- | ----- | --- | --- | --- |
16
|     | docker | run | -d  | \   |     |     |     |     |
| --- | ------ | --- | --- | --- | --- | --- | --- | --- |
17
| 18  | -v     | mes-donnees:/var/lib/mysql |     |     |     |     | \   |     |
| --- | ------ | -------------------------- | --- | --- | --- | --- | --- | --- |
|     | --name | mon-mysql                  |     |     | \   |     |     |     |
19
mysql:8.0
20
21
|     | # Monter | un  | repertoire |     |     | de l’hote | (bind mount) |     |
| --- | -------- | --- | ---------- | --- | --- | --------- | ------------ | --- |
22
|     | docker | run | -d  | \   |     |     |     |     |
| --- | ------ | --- | --- | --- | --- | --- | --- | --- |
23
| 24  | -v     | /home/user/data:/app/data |     |     |     |     | \   |     |
| --- | ------ | ------------------------- | --- | --- | --- | --- | --- | --- |
|     | --name | mon-app                   |     | \   |     |     |     |     |
25
monapp:latest
26
27
| 28  | # Monter | en  | lecture |     | seule |     |     |     |
| --- | -------- | --- | ------- | --- | ----- | --- | --- | --- |
|     | docker   | run | -d      | \   |       |     |     |     |
29
|     | -v  | /home/user/config:/app/config:ro |     |     |     |     | \   |     |
| --- | --- | -------------------------------- | --- | --- | --- | --- | --- | --- |
30
| 31  | --name | mon-app |     | \   |     |     |     |     |
| --- | ------ | ------- | --- | --- | --- | --- | --- | --- |
monapp:latest
32
33
|     | # Volume | temporaire |     |     | en  | memoire | (tmpfs) |     |
| --- | -------- | ---------- | --- | --- | --- | ------- | ------- | --- |
34
| 35  | docker  | run | -d                  | \   |     |     |     |     |
| --- | ------- | --- | ------------------- | --- | --- | --- | --- | --- |
|     | --tmpfs |     | /app/temp:size=100m |     |     |     | \   |     |
36
|     | --name | mon-app |     | \   |     |     |     |     |
| --- | ------ | ------- | --- | --- | --- | --- | --- | --- |
37
38 monapp:latest
|     |     |        |     | Listing |     | 5.8 – Gestion | des volumes | Docker |
| --- | --- | ------ | --- | ------- | --- | ------------- | ----------- | ------ |
| 5.8 |     | Docker |     | Compose |     |               |             |        |
Docker Compose permet de définir et de gérer des applications multi-conteneurs.
|     | version: |     | ’3.9’ |     |     |     |     |     |
| --- | -------- | --- | ----- | --- | --- | --- | --- | --- |
1
2
3 networks:
frontend:
4
31

| Module | DevOps  |        |     |     |     |     | S8-SIIA |
| ------ | ------- | ------ | --- | --- | --- | --- | ------- |
|        | driver: | bridge |     |     |     |     |         |
5
6 backend:
|     | driver: | bridge |     |     |     |     |     |
| --- | ------- | ------ | --- | --- | --- | --- | --- |
7
|     | internal: | true |     |     |     |     |     |
| --- | --------- | ---- | --- | --- | --- | --- | --- |
8
9
volumes:
10
db-data:
11
redis-data:
12
13 app-logs:
14
services:
15
| 16  | # Service | base | de donnees |     |     |     |     |
| --- | --------- | ---- | ---------- | --- | --- | --- | --- |
db:
17
|     | image: | postgres:15-alpine |     |     |     |     |     |
| --- | ------ | ------------------ | --- | --- | --- | --- | --- |
18
|     | container_name: |     | postgres |     |     |     |     |
| --- | --------------- | --- | -------- | --- | --- | --- | --- |
19
| 20  | restart: | unless-stopped |     |     |     |     |     |
| --- | -------- | -------------- | --- | --- | --- | --- | --- |
environment:
21
|     | POSTGRES_DB: |     | mabase |     |     |     |     |
| --- | ------------ | --- | ------ | --- | --- | --- | --- |
22
| 23  | POSTGRES_USER:     |     | ${DB_USER:-admin} |                            |     |     |         |
| --- | ------------------ | --- | ----------------- | -------------------------- | --- | --- | ------- |
|     | POSTGRES_PASSWORD: |     |                   | ${DB_PASSWORD:?DB_PASSWORD |     |     | requis} |
24
volumes:
25
- db-data:/var/lib/postgresql/data
26
- ./init.sql:/docker-entrypoint-initdb.d/init.sql:ro
27
networks:
28
- backend
29
| 30  | healthcheck: |               |     |             |     |                        |     |
| --- | ------------ | ------------- | --- | ----------- | --- | ---------------------- | --- |
|     | test:        | ["CMD-SHELL", |     | "pg_isready |     | -U $${POSTGRES_USER}"] |     |
31
|     | interval: |     | 10s |     |     |     |     |
| --- | --------- | --- | --- | --- | --- | --- | --- |
32
| 33  | timeout: | 5s  |     |     |     |     |     |
| --- | -------- | --- | --- | --- | --- | --- | --- |
|     | retries: | 5   |     |     |     |     |     |
34
35
|     | # Service | cache |     |     |     |     |     |
| --- | --------- | ----- | --- | --- | --- | --- | --- |
36
37 redis:
|     | image: | redis:7-alpine |     |     |     |     |     |
| --- | ------ | -------------- | --- | --- | --- | --- | --- |
38
|     | container_name: |     | redis |     |     |     |     |
| --- | --------------- | --- | ----- | --- | --- | --- | --- |
39
| 40  | restart: | unless-stopped |     |               |     |                   |     |
| --- | -------- | -------------- | --- | ------------- | --- | ----------------- | --- |
|     | command: | redis-server   |     | --requirepass |     | ${REDIS_PASSWORD} |     |
41
volumes:
42
- redis-data:/data
43
| 44  | networks: |     |     |     |     |     |     |
| --- | --------- | --- | --- | --- | --- | --- | --- |
- backend
45
healthcheck:
46
| 47  | test:     | ["CMD", | "redis-cli", |     | "ping"] |     |     |
| --- | --------- | ------- | ------------ | --- | ------- | --- | --- |
|     | interval: |         | 10s          |     |         |     |     |
48
49
|     | # Service | application |     |     |     |     |     |
| --- | --------- | ----------- | --- | --- | --- | --- | --- |
50
51 app:
build:
52
|     | context: | .   |     |     |     |     |     |
| --- | -------- | --- | --- | --- | --- | --- | --- |
53
| 54  | dockerfile: |     | Dockerfile |     |     |     |     |
| --- | ----------- | --- | ---------- | --- | --- | --- | --- |
args:
55
32

Module DevOps S8-SIIA
| APP_VERSION: |     | ${APP_VERSION:-1.0.0} |     |     |
| ------------ | --- | --------------------- | --- | --- |
56
| 57 image:       | monapp:${APP_VERSION:-latest} |         |     |     |
| --------------- | ----------------------------- | ------- | --- | --- |
| container_name: |                               | mon-app |     |     |
58
| restart: | unless-stopped |     |     |     |
| -------- | -------------- | --- | --- | --- |
59
60 environment:
| DATABASE_URL: |     | postgresql://admin:${DB_PASSWORD}@db:5432/ |     |     |
| ------------- | --- | ------------------------------------------ | --- | --- |
61
mabase
| REDIS_URL: |     | redis://:${REDIS_PASSWORD}@redis:6379 |     |     |
| ---------- | --- | ------------------------------------- | --- | --- |
62
63 volumes:
- app-logs:/app/logs
64
ports:
65
| 66 - "8080:8080" |     |     |     |     |
| ---------------- | --- | --- | --- | --- |
depends_on:
67
db:
68
| condition: |     | service_healthy |     |     |
| ---------- | --- | --------------- | --- | --- |
69
| 70 redis:  |     |                 |     |     |
| ---------- | --- | --------------- | --- | --- |
| condition: |     | service_healthy |     |     |
71
networks:
72
| 73 - frontend |     |     |     |     |
| ------------- | --- | --- | --- | --- |
- backend
74
deploy:
75
resources:
76
limits:
77
cpus: ’1’
78
|     | memory: | 512M |     |     |
| --- | ------- | ---- | --- | --- |
79
80
| # Service | proxy | inverse |     |     |
| --------- | ----- | ------- | --- | --- |
81
nginx:
82
| 83 image:       | nginx:alpine |       |     |     |
| --------------- | ------------ | ----- | --- | --- |
| container_name: |              | nginx |     |     |
84
| restart: | unless-stopped |     |     |     |
| -------- | -------------- | --- | --- | --- |
85
ports:
86
| 87 - "80:80" |     |     |     |     |
| ------------ | --- | --- | --- | --- |
- "443:443"
88
volumes:
89
| 90 - ./nginx/nginx.conf:/etc/nginx/nginx.conf:ro |     |     |     |     |
| ------------------------------------------------ | --- | --- | --- | --- |
- ./nginx/ssl:/etc/nginx/ssl:ro
91
depends_on:
92
- app
93
94 networks:
- frontend
95
|            | Listing  | 5.9 – Exemple | complet        | de docker-compose.yml |
| ---------- | -------- | ------------- | -------------- | --------------------- |
| # Demarrer | tous les | services      | (arriere-plan) |                       |
1
| docker compose | up  | -d  |     |     |
| -------------- | --- | --- | --- | --- |
2
3
| # Demarrer | en reconstruisant |     | les images |     |
| ---------- | ----------------- | --- | ---------- | --- |
4
| docker compose | up  | -d --build |     |     |
| -------------- | --- | ---------- | --- | --- |
5
6
| 7 # Demarrer   | un service | specifique |     |     |
| -------------- | ---------- | ---------- | --- | --- |
| docker compose | up         | -d app     |     |     |
8
33

Module DevOps S8-SIIA
9
# Arreter tous les services
10
docker compose down
11
12
# Arreter et supprimer les volumes
13
docker compose down -v
14
15
# Lister les conteneurs du projet
16
docker compose ps
17
18
# Afficher les logs de tous les services
19
docker compose logs
20
21
# Suivre les logs d’un service specifique
22
docker compose logs -f app
23
24
# Executer une commande dans un service
25
docker compose exec app /bin/bash
26
docker compose exec db psql -U admin -d mabase
27
28
# Mettre a l’echelle un service
29
docker compose scale app=3
30
31
# Afficher les processus
32
docker compose top
33
34
# Afficher la configuration fusionnee
35
docker compose config
36
37
# Valider le fichier compose
38
docker compose config --quiet
39
40
# Redemarrer un service specifique
41
docker compose restart app
42
43
# Reconstruire les images sans demarrer
44
docker compose build
45
46
# Tirer les dernieres images
47
docker compose pull
48
49
# Supprimer les conteneurs arretes
50
docker compose rm
51
52
# Afficher les differentes versions de la configuration
53
docker compose -f docker-compose.yml \
54
-f docker-compose.override.yml \
55
config
56
Listing 5.10 – Commandes Docker Compose
34

| Chapitre         |     |     | 6   |     |      |     |            |     |     |     |
| ---------------- | --- | --- | --- | --- | ---- | --- | ---------- | --- | --- | --- |
| Orchestration    |     |     |     |     | avec |     | Kubernetes |     |     |     |
| 6.1 Introduction |     |     |     |     |      |     |            |     |     |     |
Kubernetes (K8s) : système d’orchestration de conteneurs open-source développé
par Google. Il automatise le déploiement, la mise à l’échelle, la gestion de la haute
| disponibilité    |            | et les | mises | à jour  | des        | applications |          | conteneurisées. |          |        |
| ---------------- | ---------- | ------ | ----- | ------- | ---------- | ------------ | -------- | --------------- | -------- | ------ |
| 6.2 Architecture |            |        |       | de      | Kubernetes |              |          |                 |          |        |
| 6.2.1            | Composants |        |       | du Plan |            | de           | Contrôle |                 | (Control | Plane) |
— kube-apiserver : point d’entrée de toutes les requêtes API.
| — etcd           | : base | de  | données | clé-valeur |          | stockant |       | l’état du | cluster. |     |
| ---------------- | ------ | --- | ------- | ---------- | -------- | -------- | ----- | --------- | -------- | --- |
| — kube-scheduler |        |     | :       | affecte    | les Pods | aux      | nœuds | workers.  |          |     |
— kube-controller-manager : gère les boucles de contrôle (ReplicaSet, etc.).
— cloud-controller-manager : interface avec le fournisseur cloud.
| 6.2.2 | Composants |     |     | des | Nœuds |     | Workers |     |     |     |
| ----- | ---------- | --- | --- | --- | ----- | --- | ------- | --- | --- | --- |
— kubelet : agent qui s’assure que les conteneurs s’exécutent dans un Pod.
| — kube-proxy     |     |         | : maintient | les       | règles        | réseau     |     | sur les   | nœuds. |     |
| ---------------- | --- | ------- | ----------- | --------- | ------------- | ---------- | --- | --------- | ------ | --- |
| — Container      |     | Runtime |             | : Docker, |               | containerd |     | ou CRI-O. |        |     |
| 6.3 Installation |     |         |             | et        | Configuration |            |     | (kubectl) |        |     |
# Linux
1
| 2 curl -LO | "https://dl.k8s.io/release/$(curl |     |     |     |     |     |     |     | -L -s | \   |
| ---------- | --------------------------------- | --- | --- | --- | --- | --- | --- | --- | ----- | --- |
https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
3
| sudo install |     | -o  | root | -g  | root | -m  | 0755 | kubectl | /usr/local/bin/ |     |
| ------------ | --- | --- | ---- | --- | ---- | --- | ---- | ------- | --------------- | --- |
4
kubectl
5
| # Verifier |     | l’installation |     |     |     |     |     |     |     |     |
| ---------- | --- | -------------- | --- | --- | --- | --- | --- | --- | --- | --- |
6
| kubectl | version |     | --client |     |     |     |     |     |     |     |
| ------- | ------- | --- | -------- | --- | --- | --- | --- | --- | --- | --- |
7
35

Module DevOps S8-SIIA
8
# Configurer la completion bash
9
echo ’source <(kubectl completion bash)’ >> ~/.bashrc
10
source ~/.bashrc
11
12
# Alias recommandes
13
alias k=’kubectl’
14
alias kgp=’kubectl get pods’
15
alias kgs=’kubectl get services’
16
alias kgd=’kubectl get deployments’
17
Listing 6.1 – Installation de kubectl
# Afficher la configuration courante
1
kubectl config view
2
3
# Afficher le contexte actif
4
kubectl config current-context
5
6
# Lister les contextes disponibles
7
kubectl config get-contexts
8
9
# Changer de contexte
10
kubectl config use-context mon-cluster-prod
11
12
# Definir le namespace par defaut pour un contexte
13
kubectl config set-context --current --namespace=mon-namespace
14
15
# Fusionner plusieurs kubeconfig
16
KUBECONFIG=~/.kube/config:~/.kube/config-prod \
17
kubectl config view --flatten > ~/.kube/config-merge
18
Listing 6.2 – Gestion de la configuration (kubeconfig)
6.4 Ressources Fondamentales
6.4.1 Namespace
# Lister les namespaces
1
kubectl get namespaces
2
kubectl get ns
3
4
# Creer un namespace
5
kubectl create namespace dev
6
kubectl create namespace staging
7
kubectl create namespace production
8
9
# Supprimer un namespace (et toutes ses ressources)
10
kubectl delete namespace dev
11
12
# Deployer dans un namespace specifique
13
36

| Module  | DevOps |     |                 |     | S8-SIIA    |
| ------- | ------ | --- | --------------- | --- | ---------- |
| kubectl | apply  | -f  | deployment.yaml |     | -n staging |
14
15
| # Travailler |     | dans | un namespace |     | specifique |
| ------------ | --- | ---- | ------------ | --- | ---------- |
16
| kubectl | -n  | staging | get pods |     |     |
| ------- | --- | ------- | -------- | --- | --- |
17
|             |     |     | Listing | 6.3 – Gestion | des Namespaces |
| ----------- | --- | --- | ------- | ------------- | -------------- |
| 6.4.2       | Pod |     |         |               |                |
| apiVersion: |     | v1  |         |               |                |
1
| kind: | Pod |     |     |     |     |
| ----- | --- | --- | --- | --- | --- |
2
3 metadata:
| name: | mon-pod |     |     |     |     |
| ----- | ------- | --- | --- | --- | --- |
4
| namespace: |     | default |     |     |     |
| ---------- | --- | ------- | --- | --- | --- |
5
6 labels:
app: monapp
7
|     | version: | "1.0" |     |     |     |
| --- | -------- | ----- | --- | --- | --- |
8
spec:
9
containers:
10
| -   | name: monapp |     |     |     |     |
| --- | ------------ | --- | --- | --- | --- |
11
image: monapp:1.0.0
12
| 13  | ports:           |     |      |     |     |
| --- | ---------------- | --- | ---- | --- | --- |
|     | - containerPort: |     | 8080 |     |     |
14
env:
15
| 16  | - name: | APP_ENV      |     |     |     |
| --- | ------- | ------------ | --- | --- | --- |
|     | value:  | "production" |     |     |     |
17
|     | - name: | DB_PASSWORD |     |     |     |
| --- | ------- | ----------- | --- | --- | --- |
18
valueFrom:
19
| 20  | secretKeyRef: |     |           |     |     |
| --- | ------------- | --- | --------- | --- | --- |
|     | name:         |     | db-secret |     |     |
21
|     | key: |     | password |     |     |
| --- | ---- | --- | -------- | --- | --- |
22
| 23  | resources: |     |     |     |     |
| --- | ---------- | --- | --- | --- | --- |
requests:
24
|     | memory: |     | "128Mi" |     |     |
| --- | ------- | --- | ------- | --- | --- |
25
|     | cpu: | "250m" |     |     |     |
| --- | ---- | ------ | --- | --- | --- |
26
| 27  | limits: |     |         |     |     |
| --- | ------- | --- | ------- | --- | --- |
|     | memory: |     | "512Mi" |     |     |
28
|     | cpu: | "1000m" |     |     |     |
| --- | ---- | ------- | --- | --- | --- |
29
| 30  | livenessProbe: |     |     |     |     |
| --- | -------------- | --- | --- | --- | --- |
httpGet:
31
|     | path: | /health |     |     |     |
| --- | ----- | ------- | --- | --- | --- |
32
|     | port: | 8080 |     |     |     |
| --- | ----- | ---- | --- | --- | --- |
33
| 34  | initialDelaySeconds: |     |     | 30  |     |
| --- | -------------------- | --- | --- | --- | --- |
|     | periodSeconds:       |     | 10  |     |     |
35
readinessProbe:
36
| 37  | httpGet: |        |     |     |     |
| --- | -------- | ------ | --- | --- | --- |
|     | path:    | /ready |     |     |     |
38
|     | port: | 8080 |     |     |     |
| --- | ----- | ---- | --- | --- | --- |
39
|     | initialDelaySeconds: |     |     | 5   |     |
| --- | -------------------- | --- | --- | --- | --- |
40
|     | periodSeconds: |     | 5   |     |     |
| --- | -------------- | --- | --- | --- | --- |
41
| restartPolicy: |     |     | Always |     |     |
| -------------- | --- | --- | ------ | --- | --- |
42
37

Module DevOps S8-SIIA
Listing 6.4 – Manifeste d’un Pod
# Lister les pods dans le namespace courant
1
kubectl get pods
2
kubectl get pods -o wide # avec IP et noeud
3
kubectl get pods --all-namespaces # tous les namespaces
4
kubectl get pods -n mon-namespace
5
6
# Creer un pod a partir d’un manifeste
7
kubectl apply -f pod.yaml
8
9
# Decrire un pod (evenements, configuration)
10
kubectl describe pod mon-pod
11
12
# Afficher les logs d’un pod
13
kubectl logs mon-pod
14
15
# Logs d’un conteneur specifique dans un pod multi-conteneurs
16
kubectl logs mon-pod -c nom-conteneur
17
18
# Suivre les logs en temps reel
19
kubectl logs -f mon-pod
20
21
# Logs des 100 dernieres lignes
22
kubectl logs --tail=100 mon-pod
23
24
# Executer une commande dans un pod
25
kubectl exec -it mon-pod -- /bin/bash
26
kubectl exec mon-pod -- ls /app
27
28
# Copier des fichiers
29
kubectl cp mon-pod:/app/logs/app.log ./app.log
30
kubectl cp ./config.yaml mon-pod:/app/config/
31
32
# Supprimer un pod
33
kubectl delete pod mon-pod
34
35
# Supprimer a partir du manifeste
36
kubectl delete -f pod.yaml
37
38
# Forcer la suppression
39
kubectl delete pod mon-pod --force --grace-period=0
40
41
# Afficher les ressources consommees
42
kubectl top pod mon-pod
43
44
# Relancer un pod (supprime et recr e)
45
kubectl rollout restart deployment mon-deployment
46
Listing 6.5 – Commandes de gestion des Pods
38

| Module      | DevOps     |         |     | S8-SIIA |
| ----------- | ---------- | ------- | --- | ------- |
| 6.4.3       | Deployment |         |     |         |
| apiVersion: |            | apps/v1 |     |         |
1
| 2 kind: | Deployment |     |     |     |
| ------- | ---------- | --- | --- | --- |
metadata:
3
| name: | monapp |     |     |     |
| ----- | ------ | --- | --- | --- |
4
| namespace: |     | production |     |     |
| ---------- | --- | ---------- | --- | --- |
5
6 labels:
app: monapp
7
spec:
8
| 9 replicas: |     | 3   |     |     |
| ----------- | --- | --- | --- | --- |
selector:
10
matchLabels:
11
app: monapp
12
13 strategy:
type: RollingUpdate
14
rollingUpdate:
15
| 16  | maxSurge:       | 1   |     |     |
| --- | --------------- | --- | --- | --- |
|     | maxUnavailable: |     | 0   |     |
17
template:
18
metadata:
19
| 20  | labels: |        |     |     |
| --- | ------- | ------ | --- | --- |
|     | app:    | monapp |     |     |
21
|     | version: | "2.0" |     |     |
| --- | -------- | ----- | --- | --- |
22
| 23  | spec: |     |     |     |
| --- | ----- | --- | --- | --- |
affinity:
24
podAntiAffinity:
25
preferredDuringSchedulingIgnoredDuringExecution:
26
| 27  | -   | weight: | 100 |     |
| --- | --- | ------- | --- | --- |
podAffinityTerm:
28
labelSelector:
29
| 30  |     | matchExpressions: |      |     |
| --- | --- | ----------------- | ---- | --- |
|     |     | -                 | key: | app |
31
|     |     |     | operator: | In  |
| --- | --- | --- | --------- | --- |
32
values:
33
|     |     |     | - monapp |     |
| --- | --- | --- | -------- | --- |
34
|     |     | topologyKey: |     | kubernetes.io/hostname |
| --- | --- | ------------ | --- | ---------------------- |
35
containers:
36
| 37  | - name: | monapp       |     |     |
| --- | ------- | ------------ | --- | --- |
|     | image:  | monapp:2.0.0 |     |     |
38
ports:
39
| 40  | - containerPort: |     |     | 8080 |
| --- | ---------------- | --- | --- | ---- |
resources:
41
requests:
42
|     |     | memory: | "256Mi" |     |
| --- | --- | ------- | ------- | --- |
43
| 44  |     | cpu: "500m" |     |     |
| --- | --- | ----------- | --- | --- |
limits:
45
|     |     | memory: | "1Gi" |     |
| --- | --- | ------- | ----- | --- |
46
| 47  |     | cpu: "2000m" |     |     |
| --- | --- | ------------ | --- | --- |
livenessProbe:
48
httpGet:
49
path: /actuator/health/liveness
50
39

Module DevOps S8-SIIA
port: 8080
51
initialDelaySeconds: 60
52
periodSeconds: 15
53
failureThreshold: 3
54
readinessProbe:
55
httpGet:
56
path: /actuator/health/readiness
57
port: 8080
58
initialDelaySeconds: 30
59
periodSeconds: 10
60
terminationGracePeriodSeconds: 30
61
Listing 6.6 – Manifeste d’un Deployment
# Lister les deployments
1
kubectl get deployments
2
kubectl get deploy -n production
3
4
# Creer/mettre a jour un deployment
5
kubectl apply -f deployment.yaml
6
7
# Decrire un deployment
8
kubectl describe deployment monapp
9
10
# Mettre a jour l’image d’un deployment
11
kubectl set image deployment/monapp monapp=monapp:3.0.0
12
13
# Mettre a l’echelle (scaling)
14
kubectl scale deployment monapp --replicas=5
15
16
# Autoscaling horizontal
17
kubectl autoscale deployment monapp \
18
--min=2 --max=10 --cpu-percent=70
19
20
# Voir l’historique des rollouts
21
kubectl rollout history deployment monapp
22
23
# Voir les details d’une revision specifique
24
kubectl rollout history deployment monapp --revision=2
25
26
# Verifier le statut d’un rollout
27
kubectl rollout status deployment monapp
28
29
# Annuler le dernier rollout
30
kubectl rollout undo deployment monapp
31
32
# Revenir a une revision specifique
33
kubectl rollout undo deployment monapp --to-revision=3
34
35
# Mettre en pause un rollout
36
kubectl rollout pause deployment monapp
37
38
40

| Module | DevOps    |     |     |         |     |       |     | S8-SIIA |
| ------ | --------- | --- | --- | ------- | --- | ----- | --- | ------- |
| #      | Reprendre |     | un  | rollout | en  | pause |     |         |
39
| 40 kubectl |     | rollout |     | resume | deployment |     | monapp |     |
| ---------- | --- | ------- | --- | ------ | ---------- | --- | ------ | --- |
41
| #   | Supprimer |     | un  | deployment |     |     |     |     |
| --- | --------- | --- | --- | ---------- | --- | --- | --- | --- |
42
| 43 kubectl |         | delete  |           | deployment |                 | monapp |             |                 |
| ---------- | ------- | ------- | --------- | ---------- | --------------- | ------ | ----------- | --------------- |
|            |         |         | Listing   |            | 6.7 – Commandes |        | de gestion  | des Deployments |
| 6.4.4      |         | Service |           |            |                 |        |             |                 |
| #          | Service |         | ClusterIP |            | (interne        |        | au cluster) |                 |
1
| 2 apiVersion: |     |         | v1  |     |     |     |     |     |
| ------------- | --- | ------- | --- | --- | --- | --- | --- | --- |
| kind:         |     | Service |     |     |     |     |     |     |
3
metadata:
4
| 5   | name: | monapp-clusterip |     |     |     |     |     |     |
| --- | ----- | ---------------- | --- | --- | --- | --- | --- | --- |
spec:
6
|     | type: | ClusterIP |     |     |     |     |     |     |
| --- | ----- | --------- | --- | --- | --- | --- | --- | --- |
7
selector:
8
app: monapp
9
ports:
10
|     | - port: |     | 80  |     |     |     |     |     |
| --- | ------- | --- | --- | --- | --- | --- | --- | --- |
11
| 12  | targetPort: |     |     | 8080 |     |     |     |     |
| --- | ----------- | --- | --- | ---- | --- | --- | --- | --- |
13
---
14
15 # Service NodePort (accessible depuis l’exterieur via noeud)
| apiVersion: |     |     | v1  |     |     |     |     |     |
| ----------- | --- | --- | --- | --- | --- | --- | --- | --- |
16
| kind: |     | Service |     |     |     |     |     |     |
| ----- | --- | ------- | --- | --- | --- | --- | --- | --- |
17
metadata:
18
| 19  | name: | monapp-nodeport |     |     |     |     |     |     |
| --- | ----- | --------------- | --- | --- | --- | --- | --- | --- |
spec:
20
|     | type: | NodePort |     |     |     |     |     |     |
| --- | ----- | -------- | --- | --- | --- | --- | --- | --- |
21
22 selector:
app: monapp
23
ports:
24
|     | - port: |     | 80  |     |     |     |     |     |
| --- | ------- | --- | --- | --- | --- | --- | --- | --- |
25
| 26  | targetPort: |     |     | 8080  |     |      |        |                     |
| --- | ----------- | --- | --- | ----- | --- | ---- | ------ | ------------------- |
|     | nodePort:   |     |     | 30080 | #   | Port | sur le | noeud (30000-32767) |
27
28
29 ---
| #   | Service |     | LoadBalancer |     | (cloud |     | provider) |     |
| --- | ------- | --- | ------------ | --- | ------ | --- | --------- | --- |
30
| apiVersion: |     |     | v1  |     |     |     |     |     |
| ----------- | --- | --- | --- | --- | --- | --- | --- | --- |
31
| kind: |     | Service |     |     |     |     |     |     |
| ----- | --- | ------- | --- | --- | --- | --- | --- | --- |
32
33 metadata:
|     | name: | monapp-lb |     |     |     |     |     |     |
| --- | ----- | --------- | --- | --- | --- | --- | --- | --- |
34
spec:
35
| 36  | type: | LoadBalancer |     |     |     |     |     |     |
| --- | ----- | ------------ | --- | --- | --- | --- | --- | --- |
selector:
37
app: monapp
38
ports:
39
|     | - port: |     | 80  |     |     |     |     |     |
| --- | ------- | --- | --- | --- | --- | --- | --- | --- |
40
|     | targetPort: |     |     | 8080 |     |     |     |     |
| --- | ----------- | --- | --- | ---- | --- | --- | --- | --- |
41
41

| Module DevOps |     |          |     |     |         |     |          | S8-SIIA    |
| ------------- | --- | -------- | --- | --- | ------- | --- | -------- | ---------- |
|               |     | Listing  |     | 6.8 | – Types | de  | Services | Kubernetes |
| # Lister      | les | services |     |     |         |     |          |            |
1
| kubectl | get | services |     |     |     |     |     |     |
| ------- | --- | -------- | --- | --- | --- | --- | --- | --- |
2
| 3 kubectl | get | svc |     |     |     |     |     |     |
| --------- | --- | --- | --- | --- | --- | --- | --- | --- |
4
| # Creer | un  | service | a   | partir | d’un |     | manifeste |     |
| ------- | --- | ------- | --- | ------ | ---- | --- | --------- | --- |
5
| 6 kubectl | apply | -f  | service.yaml |     |     |     |     |     |
| --------- | ----- | --- | ------------ | --- | --- | --- | --- | --- |
7
| # Exposer | un  | deployment |     | comme |     | service |     |     |
| --------- | --- | ---------- | --- | ----- | --- | ------- | --- | --- |
8
| kubectl | expose | deployment |     |     | monapp | \   |     |     |
| ------- | ------ | ---------- | --- | --- | ------ | --- | --- | --- |
9
| 10 --type=ClusterIP |     |     | \   |     |     |     |     |     |
| ------------------- | --- | --- | --- | --- | --- | --- | --- | --- |
| --port=80           |     | \   |     |     |     |     |     |     |
11
--target-port=8080
12
13
| # Decrire | un  | service |     |     |     |     |     |     |
| --------- | --- | ------- | --- | --- | --- | --- | --- | --- |
14
| kubectl | describe |     | service |     | monapp-svc |     |     |     |
| ------- | -------- | --- | ------- | --- | ---------- | --- | --- | --- |
15
16
| # Acceder | a   | un service |     | via | port-forward |     |     | (developpement) |
| --------- | --- | ---------- | --- | --- | ------------ | --- | --- | --------------- |
17
| kubectl | port-forward |     |     | service/monapp-svc |     |     |     | 8080:80 |
| ------- | ------------ | --- | --- | ------------------ | --- | --- | --- | ------- |
18
| kubectl | port-forward |     |     | pod/mon-pod |     |     | 9090:8080 |     |
| ------- | ------------ | --- | --- | ----------- | --- | --- | --------- | --- |
19
20
| # Supprimer |     | un service |     |     |     |     |     |     |
| ----------- | --- | ---------- | --- | --- | --- | --- | --- | --- |
21
| kubectl | delete | service |     | monapp-svc |     |     |     |     |
| ------- | ------ | ------- | --- | ---------- | --- | --- | --- | --- |
22
|         |           | Listing   | 6.9 | – Commandes |     |         | de gestion | des Services |
| ------- | --------- | --------- | --- | ----------- | --- | ------- | ---------- | ------------ |
| 6.4.5   | ConfigMap |           | et  | Secret      |     |         |            |              |
| # Creer | un        | ConfigMap |     | depuis      | des | valeurs |            |              |
1
| kubectl | create | configmap |     |     | app-config |     | \   |     |
| ------- | ------ | --------- | --- | --- | ---------- | --- | --- | --- |
2
| 3 --from-literal=APP_ENV=production |     |     |     |     |     |     | \   |     |
| ----------------------------------- | --- | --- | --- | --- | --- | --- | --- | --- |
--from-literal=LOG_LEVEL=INFO
4
5
| 6 # Creer | un     | ConfigMap |     | depuis | un           | fichier |     |     |
| --------- | ------ | --------- | --- | ------ | ------------ | ------- | --- | --- |
| kubectl   | create | configmap |     |        | nginx-config |         |     | \   |
7
--from-file=nginx.conf
8
9
| 10 # Creer | un     | ConfigMap |     | depuis | un          | repertoire |     |     |
| ---------- | ------ | --------- | --- | ------ | ----------- | ---------- | --- | --- |
| kubectl    | create | configmap |     |        | app-configs |            | \   |     |
11
--from-file=./configs/
12
13
| # Lister | les | ConfigMaps |     |     |     |     |     |     |
| -------- | --- | ---------- | --- | --- | --- | --- | --- | --- |
14
| kubectl | get | configmaps |     |     |     |     |     |     |
| ------- | --- | ---------- | --- | --- | --- | --- | --- | --- |
15
| 16 kubectl | get | cm  |     |     |     |     |     |     |
| ---------- | --- | --- | --- | --- | --- | --- | --- | --- |
17
| # Afficher |     | le contenu |     | d’un | ConfigMap |     |     |     |
| ---------- | --- | ---------- | --- | ---- | --------- | --- | --- | --- |
18
| kubectl | describe |     | configmap |     | app-config |     |     |     |
| ------- | -------- | --- | --------- | --- | ---------- | --- | --- | --- |
19
| 20 kubectl | get | configmap |     | app-config |     | -o  | yaml |     |
| ---------- | --- | --------- | --- | ---------- | --- | --- | ---- | --- |
21
42

| Module DevOps |     |        |        |     |     |     |     | S8-SIIA |
| ------------- | --- | ------ | ------ | --- | --- | --- | --- | ------- |
| # Creer       | un  | Secret | opaque |     |     |     |     |         |
22
| 23 kubectl                    | create |     | secret | generic | db-secret |     | \   |     |
| ----------------------------- | ------ | --- | ------ | ------- | --------- | --- | --- | --- |
| --from-literal=username=admin |        |     |        |         |           | \   |     |     |
24
--from-literal=password=MonMotDePasse123!
25
26
| # Creer | un  | Secret | depuis | un  | fichier |     |     |     |
| ------- | --- | ------ | ------ | --- | ------- | --- | --- | --- |
27
| kubectl | create |     | secret | generic | tls-secret |     |     | \   |
| ------- | ------ | --- | ------ | ------- | ---------- | --- | --- | --- |
28
| --from-file=tls.crt=./certs/server.crt |     |     |     |     |     |     |     | \   |
| -------------------------------------- | --- | --- | --- | --- | --- | --- | --- | --- |
29
30 --from-file=tls.key=./certs/server.key
31
| # Secret | de  | type | TLS |     |     |     |     |     |
| -------- | --- | ---- | --- | --- | --- | --- | --- | --- |
32
| 33 kubectl                | create |     | secret | tls | mon-tls | \   |     |     |
| ------------------------- | ------ | --- | ------ | --- | ------- | --- | --- | --- |
| --cert=./certs/server.crt |        |     |        |     | \       |     |     |     |
34
--key=./certs/server.key
35
36
| 37 # Secret | de     | type | Docker | Registry        |     |     |         |     |
| ----------- | ------ | ---- | ------ | --------------- | --- | --- | ------- | --- |
| kubectl     | create |      | secret | docker-registry |     |     | regcred | \   |
38
| --docker-server=registry.exemple.com |     |     |     |     |     |     | \   |     |
| ------------------------------------ | --- | --- | --- | --- | --- | --- | --- | --- |
39
| 40 --docker-username=mon-user |     |     |     |     | \   |     |     |     |
| ----------------------------- | --- | --- | --- | --- | --- | --- | --- | --- |
| --docker-password=mon-mdp     |     |     |     |     | \   |     |     |     |
41
--docker-email=contact@exemple.com
42
43
| # Lister | les | secrets |     |     |     |     |     |     |
| -------- | --- | ------- | --- | --- | --- | --- | --- | --- |
44
| kubectl | get | secrets |     |     |     |     |     |     |
| ------- | --- | ------- | --- | --- | --- | --- | --- | --- |
45
46
| 47 # Decoder |     | un secret |     | (base64) |     |     |     |     |
| ------------ | --- | --------- | --- | -------- | --- | --- | --- | --- |
kubectl get secret db-secret -o jsonpath=’{.data.password}’ |
48
| base64 |     | -d  |     |     |     |     |     |     |
| ------ | --- | --- | --- | --- | --- | --- | --- | --- |
49
| # Supprimer |     | un  | ConfigMap | /   | Secret |     |     |     |
| ----------- | --- | --- | --------- | --- | ------ | --- | --- | --- |
50
| kubectl | delete |     | configmap | app-config |     |     |     |     |
| ------- | ------ | --- | --------- | ---------- | --- | --- | --- | --- |
51
| kubectl | delete |     | secret | db-secret |     |     |     |     |
| ------- | ------ | --- | ------ | --------- | --- | --- | --- | --- |
52
|                    |                  | Listing |      | 6.10 – Gestion | des                   | ConfigMaps |     | et Secrets |
| ------------------ | ---------------- | ------- | ---- | -------------- | --------------------- | ---------- | --- | ---------- |
| 6.4.6              | PersistentVolume |         |      | et             | PersistentVolumeClaim |            |     |            |
| # PersistentVolume |                  |         | (PV) |                |                       |            |     |            |
1
| 2 apiVersion: |                  | v1  |     |     |     |     |     |     |
| ------------- | ---------------- | --- | --- | --- | --- | --- | --- | --- |
| kind:         | PersistentVolume |     |     |     |     |     |     |     |
3
metadata:
4
| name: | mon-pv |     |     |     |     |     |     |     |
| ----- | ------ | --- | --- | --- | --- | --- | --- | --- |
5
6 spec:
capacity:
7
storage: 10Gi
8
| 9 volumeMode: |     | Filesystem |     |     |     |     |     |     |
| ------------- | --- | ---------- | --- | --- | --- | --- | --- | --- |
accessModes:
10
- ReadWriteOnce
11
| persistentVolumeReclaimPolicy: |     |     |     |     |     | Retain |     |     |
| ------------------------------ | --- | --- | --- | --- | --- | ------ | --- | --- |
12
| storageClassName: |     |     |     | standard |     |     |     |     |
| ----------------- | --- | --- | --- | -------- | --- | --- | --- | --- |
13
hostPath:
14
43

| Module | DevOps |     |     | S8-SIIA |
| ------ | ------ | --- | --- | ------- |
path: /mnt/data
15
16
---
17
| # PersistentVolumeClaim |     |     | (PVC) |     |
| ----------------------- | --- | --- | ----- | --- |
18
| 19 apiVersion: |                       | v1  |     |     |
| -------------- | --------------------- | --- | --- | --- |
| kind:          | PersistentVolumeClaim |     |     |     |
20
metadata:
21
| name: | mon-pvc |     |     |     |
| ----- | ------- | --- | --- | --- |
22
23 spec:
accessModes:
24
- ReadWriteOnce
25
26 resources:
requests:
27
|     | storage: | 5Gi |     |     |
| --- | -------- | --- | --- | --- |
28
storageClassName: standard
29
|            | Listing | 6.11 – PersistentVolume |     | et PersistentVolumeClaim |
| ---------- | ------- | ----------------------- | --- | ------------------------ |
| 1 # Lister | les     | PersistentVolumes       |     |                          |
| kubectl    | get     | pv                      |     |                          |
2
3
| 4 # Lister | les | PersistentVolumeClaims |     |     |
| ---------- | --- | ---------------------- | --- | --- |
| kubectl    | get | pvc                    |     |     |
5
6
| # Decrire | un  | PVC |     |     |
| --------- | --- | --- | --- | --- |
7
| 8 kubectl | describe | pvc mon-pvc |     |     |
| --------- | -------- | ----------- | --- | --- |
9
| # Supprimer |     | un PVC |     |     |
| ----------- | --- | ------ | --- | --- |
10
| 11 kubectl  | delete  | pvc mon-pvc          |             |           |
| ----------- | ------- | -------------------- | ----------- | --------- |
|             |         | Listing 6.12         | – Commandes | PV et PVC |
| 6.4.7       | Ingress |                      |             |           |
| apiVersion: |         | networking.k8s.io/v1 |             |           |
1
| kind: | Ingress |     |     |     |
| ----- | ------- | --- | --- | --- |
2
metadata:
3
| 4 name: | mon-ingress |     |     |     |
| ------- | ----------- | --- | --- | --- |
annotations:
5
nginx.ingress.kubernetes.io/rewrite-target: /
6
| 7   | nginx.ingress.kubernetes.io/ssl-redirect: |     |     | "true" |
| --- | ----------------------------------------- | --- | --- | ------ |
spec:
8
ingressClassName: nginx
9
tls:
10
| 11 - | hosts: |     |     |     |
| ---- | ------ | --- | --- | --- |
- app.exemple.com
12
|     | secretName: | mon-tls |     |     |
| --- | ----------- | ------- | --- | --- |
13
14 rules:
| -   | host: app.exemple.com |     |     |     |
| --- | --------------------- | --- | --- | --- |
15
http:
16
paths:
17
| 18  | - path: | /api |     |     |
| --- | ------- | ---- | --- | --- |
44

| Module DevOps |           |     |     |        |     |     | S8-SIIA |
| ------------- | --------- | --- | --- | ------ | --- | --- | ------- |
|               | pathType: |     |     | Prefix |     |     |         |
19
| 20  | backend: |     |     |     |     |     |     |
| --- | -------- | --- | --- | --- | --- | --- | --- |
service:
21
|     |     | name: |     | api-service |     |     |     |
| --- | --- | ----- | --- | ----------- | --- | --- | --- |
22
| 23  |     | port: |         |     |     |     |     |
| --- | --- | ----- | ------- | --- | --- | --- | --- |
|     |     |       | number: | 80  |     |     |     |
24
|     | - path: |     | /   |     |     |     |     |
| --- | ------- | --- | --- | --- | --- | --- | --- |
25
|     | pathType: |     |     | Prefix |     |     |     |
| --- | --------- | --- | --- | ------ | --- | --- | --- |
26
| 27  | backend: |     |     |     |     |     |     |
| --- | -------- | --- | --- | --- | --- | --- | --- |
service:
28
|     |     | name: |     | frontend-service |     |     |     |
| --- | --- | ----- | --- | ---------------- | --- | --- | --- |
29
| 30  |     | port: |         |     |     |     |     |
| --- | --- | ----- | ------- | --- | --- | --- | --- |
|     |     |       | number: | 80  |     |     |     |
31
|               |     |        |     | Listing        | 6.13 | – Manifeste | Ingress   |
| ------------- | --- | ------ | --- | -------------- | ---- | ----------- | --------- |
| 6.5 Commandes |     |        |     | Générales      |      |             | kubectl   |
| # Obtenir     |     | toutes |     | les ressources |      | d’un        | namespace |
1
| 2 kubectl | get | all | -n  | mon-namespace |     |     |     |
| --------- | --- | --- | --- | ------------- | --- | --- | --- |
3
| # Appliquer |     | des | modifications |     |     | (create | ou update) |
| ----------- | --- | --- | ------------- | --- | --- | ------- | ---------- |
4
| 5 kubectl | apply |     | -f  | manifeste.yaml |     |     |     |
| --------- | ----- | --- | --- | -------------- | --- | --- | --- |
6
| # Appliquer |     | tous |     | les manifestes |     | d’un | repertoire |
| ----------- | --- | ---- | --- | -------------- | --- | ---- | ---------- |
7
| 8 kubectl | apply |     | -f  | ./k8s/ |     |     |     |
| --------- | ----- | --- | --- | ------ | --- | --- | --- |
9
| # Voir | les | differences |     |     | avant | application |     |
| ------ | --- | ----------- | --- | --- | ----- | ----------- | --- |
10
| kubectl | diff | -f  | manifeste.yaml |     |     |     |     |
| ------- | ---- | --- | -------------- | --- | --- | --- | --- |
11
12
| # Supprimer |     | des | ressources |     |     |     |     |
| ----------- | --- | --- | ---------- | --- | --- | --- | --- |
13
| kubectl | delete |     | -f  | manifeste.yaml |     |     |     |
| ------- | ------ | --- | --- | -------------- | --- | --- | --- |
14
15
| # Obtenir |     | des | ressources |     | au  | format | JSON/YAML |
| --------- | --- | --- | ---------- | --- | --- | ------ | --------- |
16
| kubectl | get | deployment |     |     | monapp | -o  | yaml |
| ------- | --- | ---------- | --- | --- | ------ | --- | ---- |
17
| kubectl | get | pods |     | -o json |     |     |     |
| ------- | --- | ---- | --- | ------- | --- | --- | --- |
18
19
| # Filtrer |     | avec | jsonpath |     |     |     |     |
| --------- | --- | ---- | -------- | --- | --- | --- | --- |
20
| kubectl | get | pods |     | -o jsonpath=’{.items[*].metadata.name}’ |     |     |     |
| ------- | --- | ---- | --- | --------------------------------------- | --- | --- | --- |
21
22
| # Filtrer |     | avec | custom-columns |     |     |     |     |
| --------- | --- | ---- | -------------- | --- | --- | --- | --- |
23
| kubectl | get | pods |     | \   |     |     |     |
| ------- | --- | ---- | --- | --- | --- | --- | --- |
24
| -o custom-columns=NOM:.metadata.name,STATUT:.status.phase |     |     |     |     |     |     |     |
| --------------------------------------------------------- | --- | --- | --- | --- | --- | --- | --- |
25
26
| # Filtrer |     | par | label |     |     |     |     |
| --------- | --- | --- | ----- | --- | --- | --- | --- |
27
| kubectl | get | pods |     | -l app=monapp |     |     |     |
| ------- | --- | ---- | --- | ------------- | --- | --- | --- |
28
| 29 kubectl | get | pods |     | -l ’env | in  | (prod,staging)’ |     |
| ---------- | --- | ---- | --- | ------- | --- | --------------- | --- |
30
| # Etiqueter |     | une | ressource |     |     |     |     |
| ----------- | --- | --- | --------- | --- | --- | --- | --- |
31
| kubectl | label |     | pod | mon-pod | environment=production |     |     |
| ------- | ----- | --- | --- | ------- | ---------------------- | --- | --- |
32
33
45

Module DevOps S8-SIIA
# Annoter une ressource
34
kubectl annotate pod mon-pod \
35
description="Pod de production critique"
36
37
# Voir les evenements du cluster
38
kubectl get events --sort-by=’.lastTimestamp’
39
kubectl get events -n mon-namespace
40
41
# Afficher les ressources consommees par les noeuds
42
kubectl top nodes
43
44
# Afficher les ressources consommees par les pods
45
kubectl top pods
46
47
# Appliquer un correctif (patch)
48
kubectl patch deployment monapp \
49
-p ’{"spec":{"replicas":5}}’
50
51
# Editer une ressource directement
52
kubectl edit deployment monapp
53
Listing 6.14 – Commandes generales kubectl
6.6 Helm – Gestionnaire de Paquets Kubernetes
# Installer Helm
1
curl https://raw.githubusercontent.com/helm/helm/main/scripts/
2
get-helm-3 | bash
3
# Verifier la version
4
helm version
5
6
# Ajouter un depot de charts
7
helm repo add stable https://charts.helm.sh/stable
8
helm repo add bitnami https://charts.bitnami.com/bitnami
9
10
# Mettre a jour les depots
11
helm repo update
12
13
# Lister les depots
14
helm repo list
15
16
# Rechercher un chart
17
helm search repo nginx
18
19
# Afficher les valeurs par defaut d’un chart
20
helm show values bitnami/nginx
21
22
# Installer un chart
23
helm install mon-nginx bitnami/nginx
24
25
46

| Module DevOps |     |      |     |         |     |                |     | S8-SIIA |
| ------------- | --- | ---- | --- | ------- | --- | -------------- | --- | ------- |
| # Installer   |     | avec | des | valeurs |     | personnalisees |     |         |
26
| 27 helm install |                       | mon-nginx |     | bitnami/nginx |     |     | \   |     |
| --------------- | --------------------- | --------- | --- | ------------- | --- | --- | --- | --- |
| --set           | service.type=NodePort |           |     |               |     | \   |     |     |
28
| --set | replicaCount=2 |     |     | \   |     |     |     |     |
| ----- | -------------- | --- | --- | --- | --- | --- | --- | --- |
29
| 30 -n production |     |     | --create-namespace |     |     |     |     |     |
| ---------------- | --- | --- | ------------------ | --- | --- | --- | --- | --- |
31
| # Installer |     | avec | un  | fichier | de  | valeurs |     |     |
| ----------- | --- | ---- | --- | ------- | --- | ------- | --- | --- |
32
| helm install |     | mon-nginx |     | bitnami/nginx |     |     | \   |     |
| ------------ | --- | --------- | --- | ------------- | --- | --- | --- | --- |
33
| 34 -f mes-valeurs.yaml |     |     |     |     |     |     |     |     |
| ---------------------- | --- | --- | --- | --- | --- | --- | --- | --- |
35
| # Mettre | a   | jour | un  | deploiement |     | Helm |     |     |
| -------- | --- | ---- | --- | ----------- | --- | ---- | --- | --- |
36
| 37 helm upgrade |     | mon-nginx |     | bitnami/nginx |     |     | --set replicaCount=3 |     |
| --------------- | --- | --------- | --- | ------------- | --- | --- | -------------------- | --- |
38
| # Installer |     | ou mettre |     | a jour | (upsert) |     |     |     |
| ----------- | --- | --------- | --- | ------ | -------- | --- | --- | --- |
39
| helm upgrade |     | --install |     | mon-nginx |     |     | bitnami/nginx | \   |
| ------------ | --- | --------- | --- | --------- | --- | --- | ------------- | --- |
40
| 41 -f mes-valeurs.yaml |     |     |     |     |     |     |     |     |
| ---------------------- | --- | --- | --- | --- | --- | --- | --- | --- |
42
| # Lister | les | releases |     |     |     |     |     |     |
| -------- | --- | -------- | --- | --- | --- | --- | --- | --- |
43
| 44 helm list |     |            |     |     |     |     |     |     |
| ------------ | --- | ---------- | --- | --- | --- | --- | --- | --- |
| helm ls      | -n  | production |     |     |     |     |     |     |
45
46
| # Voir | l’historique |     |     | d’une | release |     |     |     |
| ------ | ------------ | --- | --- | ----- | ------- | --- | --- | --- |
47
| helm history |     | mon-nginx |     |     |     |     |     |     |
| ------------ | --- | --------- | --- | --- | --- | --- | --- | --- |
48
49
| # Revenir |     | a une | version | precedente |     |     |     |     |
| --------- | --- | ----- | ------- | ---------- | --- | --- | --- | --- |
50
| 51 helm rollback |     | mon-nginx |     | 1   |     |     |     |     |
| ---------------- | --- | --------- | --- | --- | --- | --- | --- | --- |
52
| # Desinstaller |     | une |     | release |     |     |     |     |
| -------------- | --- | --- | --- | ------- | --- | --- | --- | --- |
53
| 54 helm uninstall |     | mon-nginx |     |     |     |     |     |     |
| ----------------- | --- | --------- | --- | --- | --- | --- | --- | --- |
55
| # Creer | un  | nouveau |     | chart |     |     |     |     |
| ------- | --- | ------- | --- | ----- | --- | --- | --- | --- |
56
| helm create |     | mon-chart |     |     |     |     |     |     |
| ----------- | --- | --------- | --- | --- | --- | --- | --- | --- |
57
58
| # Valider |     | un chart |     |     |     |     |     |     |
| --------- | --- | -------- | --- | --- | --- | --- | --- | --- |
59
| helm lint |     | mon-chart/ |     |     |     |     |     |     |
| --------- | --- | ---------- | --- | --- | --- | --- | --- | --- |
60
61
| # Generer |     | le YAML | sans | deployer |     | (debug) |     |     |
| --------- | --- | ------- | ---- | -------- | --- | ------- | --- | --- |
62
| helm template |     | mon-nginx |     | bitnami/nginx |     |     | -f mes-valeurs.yaml |     |
| ------------- | --- | --------- | --- | ------------- | --- | --- | ------------------- | --- |
63
|     |     |     | Listing | 6.15 – | Commandes |     | Helm essentielles |     |
| --- | --- | --- | ------- | ------ | --------- | --- | ----------------- | --- |
47

| Chapitre         |     | 7   |     |         |     |     |
| ---------------- | --- | --- | --- | ------- | --- | --- |
| Infrastructure   |     |     |     | as Code |     |     |
| 7.1 Introduction |     |     |     |         |     |     |
Infrastructure as Code (IaC) : pratique consistant à décrire et à gérer l’infrastruc-
ture informatique (serveurs, réseaux, bases de données, etc.) sous forme de fichiers de
configuration versionnables et automatisables, plutôt que par des interventions ma-
nuelles.
| Avantages          | de           | l’IaC          | :            |                      |                 |     |
| ------------------ | ------------ | -------------- | ------------ | -------------------- | --------------- | --- |
| — Reproductibilité |              |                | et cohérence | entre les            | environnements. |     |
| — Versionnage      |              | et traçabilité |              | des modifications.   |                 |     |
| — Automatisation   |              |                | et rapidité  | de provisionnement.  |                 |     |
| — Réduction        |              | des erreurs    |              | humaines.            |                 |     |
| — Documentation    |              | vivante        |              | de l’infrastructure. |                 |     |
| 7.2 Terraform      |              |                |              |                      |                 |     |
| 7.2.1              | Présentation |                |              |                      |                 |     |
Terraform, développé par HashiCorp, est l’outil IaC le plus populaire. Il supporte des
dizaines de fournisseurs cloud (AWS, Azure, GCP, etc.) et utilise le langage HCL (Hashi-
| Corp Configuration |              | Language). |     |              |            |           |
| ------------------ | ------------ | ---------- | --- | ------------ | ---------- | --------- |
| 7.2.2              | Installation |            |     |              |            |           |
| # Methode          |              | 1 : via    | le  | gestionnaire | de paquets | HashiCorp |
1
| wget | -O- https://apt.releases.hashicorp.com/gpg |     |     |     |     | \   |
| ---- | ------------------------------------------ | --- | --- | --- | --- | --- |
2
3 | sudo gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-
keyring.gpg
4
5 echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-
| keyring.gpg] |     |     | \   |     |     |     |
| ------------ | --- | --- | --- | --- | --- | --- |
https://apt.releases.hashicorp.com $(lsb_release -cs) main" \
6
| | sudo | tee | /etc/apt/sources.list.d/hashicorp.list |     |     |     |     |
| ------ | --- | -------------------------------------- | --- | --- | --- | --- |
7
48

Module DevOps S8-SIIA
8
| 9 sudo apt-get | update |     | &&  | sudo | apt-get | install | -y terraform |
| -------------- | ------ | --- | --- | ---- | ------- | ------- | ------------ |
10
| # Verifier | l’installation |     |     |     |     |     |     |
| ---------- | -------------- | --- | --- | --- | --- | --- | --- |
11
| 12 terraform | version |     |     |     |     |     |     |
| ------------ | ------- | --- | --- | --- | --- | --- | --- |
13
| # Completion | bash |     |     |     |     |     |     |
| ------------ | ---- | --- | --- | --- | --- | --- | --- |
14
| terraform | -install-autocomplete |     |     |     |     |     |     |
| --------- | --------------------- | --- | --- | --- | --- | --- | --- |
15
|                 |     | Listing    |     | 7.1 – | Installation | de Terraform |     |
| --------------- | --- | ---------- | --- | ----- | ------------ | ------------ | --- |
| 7.2.3 Commandes |     | Terraform  |     |       |              |              |     |
| # Initialiser   | le  | repertoire |     |       | de travail   |              |     |
1
| 2 terraform | init |     |     |     |     |     |     |
| ----------- | ---- | --- | --- | --- | --- | --- | --- |
3
| # Initialiser | avec | mise |     | a jour | des | providers |     |
| ------------- | ---- | ---- | --- | ------ | --- | --------- | --- |
4
| terraform | init | -upgrade |     |     |     |     |     |
| --------- | ---- | -------- | --- | --- | --- | --- | --- |
5
6
| # Formater | le code | HCL |     |     |     |     |     |
| ---------- | ------- | --- | --- | --- | --- | --- | --- |
7
| terraform | fmt |     |     |     |     |     |     |
| --------- | --- | --- | --- | --- | --- | --- | --- |
8
9
| # Formater | recursivement |     |     |     |     |     |     |
| ---------- | ------------- | --- | --- | --- | --- | --- | --- |
10
| terraform | fmt -recursive |     |     |     |     |     |     |
| --------- | -------------- | --- | --- | --- | --- | --- | --- |
11
12
| # Valider | la syntaxe |     |     |     |     |     |     |
| --------- | ---------- | --- | --- | --- | --- | --- | --- |
13
| terraform | validate |     |     |     |     |     |     |
| --------- | -------- | --- | --- | --- | --- | --- | --- |
14
15
| 16 # Planifier | les  | modifications |     |     | (dry-run) |     |     |
| -------------- | ---- | ------------- | --- | --- | --------- | --- | --- |
| terraform      | plan |               |     |     |           |     |     |
17
18
| 19 # Sauvegarder | le   | plan                | dans | un  | fichier |     |     |
| ---------------- | ---- | ------------------- | ---- | --- | ------- | --- | --- |
| terraform        | plan | -out=monplan.tfplan |      |     |         |     |     |
20
21
| # Appliquer | les | modifications |     |     |     |     |     |
| ----------- | --- | ------------- | --- | --- | --- | --- | --- |
22
| 23 terraform | apply |     |     |     |     |     |     |
| ------------ | ----- | --- | --- | --- | --- | --- | --- |
24
| # Appliquer | un  | plan | sauvegarde |     |     |     |     |
| ----------- | --- | ---- | ---------- | --- | --- | --- | --- |
25
| 26 terraform | apply | monplan.tfplan |     |     |     |     |     |
| ------------ | ----- | -------------- | --- | --- | --- | --- | --- |
27
| # Appliquer | sans | confirmation |     |     |     |     |     |
| ----------- | ---- | ------------ | --- | --- | --- | --- | --- |
28
| terraform | apply | -auto-approve |     |     |     |     |     |
| --------- | ----- | ------------- | --- | --- | --- | --- | --- |
29
30
| # Passer | des variables |     |     |     |     |     |     |
| -------- | ------------- | --- | --- | --- | --- | --- | --- |
31
terraform apply -var="region=eu-west-1" -var="instance_count=3"
32
33
| # Appliquer | avec | fichier |     | de  | variables |     |     |
| ----------- | ---- | ------- | --- | --- | --------- | --- | --- |
34
| terraform | apply | -var-file="prod.tfvars" |     |     |     |     |     |
| --------- | ----- | ----------------------- | --- | --- | --- | --- | --- |
35
36
| # Detruire | l’infrastructure |     |     |     |     |     |     |
| ---------- | ---------------- | --- | --- | --- | --- | --- | --- |
37
| terraform | destroy |     |     |     |     |     |     |
| --------- | ------- | --- | --- | --- | --- | --- | --- |
38
49

| Module DevOps |     |     |     |     |     |     |     | S8-SIIA |
| ------------- | --- | --- | --- | --- | --- | --- | --- | ------- |
39
| 40 # Detruire | sans    | confirmation |               |     |     |     |     |     |
| ------------- | ------- | ------------ | ------------- | --- | --- | --- | --- | --- |
| terraform     | destroy |              | -auto-approve |     |     |     |     |     |
41
42
| 43 # Detruire | une     | ressource |                                  |     | specifique |     |     |     |
| ------------- | ------- | --------- | -------------------------------- | --- | ---------- | --- | --- | --- |
| terraform     | destroy |           | -target=aws_instance.mon_serveur |     |            |     |     |     |
44
45
| # Afficher | l’etat |     | actuel |     |     |     |     |     |
| ---------- | ------ | --- | ------ | --- | --- | --- | --- | --- |
46
| 47 terraform | show |     |     |     |     |     |     |     |
| ------------ | ---- | --- | --- | --- | --- | --- | --- | --- |
48
| # Lister | les | ressources |     |     | dans l’etat |     |     |     |
| -------- | --- | ---------- | --- | --- | ----------- | --- | --- | --- |
49
| 50 terraform | state | list |     |     |     |     |     |     |
| ------------ | ----- | ---- | --- | --- | --- | --- | --- | --- |
51
| # Afficher | une | ressource |     |     | specifique | dans |     | l’etat |
| ---------- | --- | --------- | --- | --- | ---------- | ---- | --- | ------ |
52
| terraform | state | show |     | aws_instance.mon_serveur |     |     |     |     |
| --------- | ----- | ---- | --- | ------------------------ | --- | --- | --- | --- |
53
54
| # Deplacer | une | ressource |     |     | dans l’etat |     |     |     |
| ---------- | --- | --------- | --- | --- | ----------- | --- | --- | --- |
55
| terraform | state | mv  | aws_instance.ancien |     |     |     | aws_instance.nouveau |     |
| --------- | ----- | --- | ------------------- | --- | --- | --- | -------------------- | --- |
56
57
| # Retirer | une | ressource |     |     | de l’etat | (sans | la  | supprimer) |
| --------- | --- | --------- | --- | --- | --------- | ----- | --- | ---------- |
58
| terraform | state | rm  | aws_instance.mon_serveur |     |     |     |     |     |
| --------- | ----- | --- | ------------------------ | --- | --- | --- | --- | --- |
59
60
| # Importer | une | ressource |     |     | existante |     |     |     |
| ---------- | --- | --------- | --- | --- | --------- | --- | --- | --- |
61
terraform import aws_instance.mon_serveur i-0123456789abcdef0
62
63
| 64 # Afficher | les    | outputs |     |     |     |     |     |     |
| ------------- | ------ | ------- | --- | --- | --- | --- | --- | --- |
| terraform     | output |         |     |     |     |     |     |     |
65
| terraform | output |     | nom_du_output |     |     |     |     |     |
| --------- | ------ | --- | ------------- | --- | --- | --- | --- | --- |
66
67
| # Graphe | de dependances |     |     |     |     |     |     |     |
| -------- | -------------- | --- | --- | --- | --- | --- | --- | --- |
68
| terraform | graph | |   | dot | -Tsvg | > graph.svg |     |     |     |
| --------- | ----- | --- | --- | ----- | ----------- | --- | --- | --- |
69
70
| 71 # Verouiller/deverrouiller |              |     |     |         | l’etat |     |     |     |
| ----------------------------- | ------------ | --- | --- | ------- | ------ | --- | --- | --- |
| terraform                     | force-unlock |     |     | LOCK_ID |        |     |     |     |
72
73
| 74 # Mettre | a jour | les     | modules |     |     |     |     |     |
| ----------- | ------ | ------- | ------- | --- | --- | --- | --- | --- |
| terraform   | get    | -update |         |     |     |     |     |     |
75
76
| # Tester | les | expressions |     |     |     |     |     |     |
| -------- | --- | ----------- | --- | --- | --- | --- | --- | --- |
77
| 78 terraform      | console |     |               |     |             |           |           |     |
| ----------------- | ------- | --- | ------------- | --- | ----------- | --------- | --------- | --- |
|                   |         |     | Listing       |     | 7.2 – Cycle | de vie    | Terraform |     |
| 7.2.4 Exemple     |         | de  | Configuration |     |             | Terraform |           |     |
| 1 # Configuration |         | du  | provider      |     |             |           |           |     |
| terraform         | {       |     |               |     |             |           |           |     |
2
| required_version |     |     | =   | ">= | 1.0" |     |     |     |
| ---------------- | --- | --- | --- | --- | ---- | --- | --- | --- |
3
| required_providers |     |     |     | {   |     |     |     |     |
| ------------------ | --- | --- | --- | --- | --- | --- | --- | --- |
4
aws = {
5
|     | source | = "hashicorp/aws" |     |     |     |     |     |     |
| --- | ------ | ----------------- | --- | --- | --- | --- | --- | --- |
6
50

| Module |     | DevOps  |     |     |      |     |     | S8-SIIA |
| ------ | --- | ------- | --- | --- | ---- | --- | --- | ------- |
|        |     | version | =   | "~> | 5.0" |     |     |         |
7
8 }
}
9
|     | backend |     | "s3" { |     |     |     |     |     |
| --- | ------- | --- | ------ | --- | --- | --- | --- | --- |
10
| 11  |     | bucket | = "mon-tfstate"                  |     |     |     |     |     |
| --- | --- | ------ | -------------------------------- | --- | --- | --- | --- | --- |
|     |     | key    | = "production/terraform.tfstate" |     |     |     |     |     |
12
|     |     | region | = "eu-west-1" |     |     |     |     |     |
| --- | --- | ------ | ------------- | --- | --- | --- | --- | --- |
13
}
14
15 }
16
|     | provider |     | "aws" { |     |     |     |     |     |
| --- | -------- | --- | ------- | --- | --- | --- | --- | --- |
17
| 18  | region       |     | = var.region |     |     |     |     |     |
| --- | ------------ | --- | ------------ | --- | --- | --- | --- | --- |
|     | default_tags |     | {            |     |     |     |     |     |
19
|     |     | tags | = { |     |     |     |     |     |
| --- | --- | ---- | --- | --- | --- | --- | --- | --- |
20
|     |     | Environment |     | =   | var.environment |     |     |     |
| --- | --- | ----------- | --- | --- | --------------- | --- | --- | --- |
21
| 22  |     | ManagedBy |     | =   | "Terraform" |     |     |     |
| --- | --- | --------- | --- | --- | ----------- | --- | --- | --- |
}
23
}
24
25 }
26
# Variables
27
|     | variable |     | "region" | {   |     |     |     |     |
| --- | -------- | --- | -------- | --- | --- | --- | --- | --- |
28
|     | type |     | = string |     |     |     |     |     |
| --- | ---- | --- | -------- | --- | --- | --- | --- | --- |
29
|     | default |     | = "eu-west-1" |     |     |     |     |     |
| --- | ------- | --- | ------------- | --- | --- | --- | --- | --- |
30
}
31
| 32  | variable |     | "environment" |     | {   |     |     |     |
| --- | -------- | --- | ------------- | --- | --- | --- | --- | --- |
|     | type     | =   | string        |     |     |     |     |     |
33
}
34
| 35  | variable |     | "instance_count" |     |     | {   |     |     |
| --- | -------- | --- | ---------------- | --- | --- | --- | --- | --- |
|     | type     |     | = number         |     |     |     |     |     |
36
|     | default |     | = 2 |     |     |     |     |     |
| --- | ------- | --- | --- | --- | --- | --- | --- | --- |
37
}
38
39
# Ressources
40
|     | resource |     | "aws_vpc" | "principal" |     |     | {   |     |
| --- | -------- | --- | --------- | ----------- | --- | --- | --- | --- |
41
| 42  | cidr_block           |     |     |     | =   | "10.0.0.0/16" |     |     |
| --- | -------------------- | --- | --- | --- | --- | ------------- | --- | --- |
|     | enable_dns_hostnames |     |     |     | =   | true          |     |     |
43
|     | tags | =   | { Name | = "vpc-${var.environment}" |     |     |     | }   |
| --- | ---- | --- | ------ | -------------------------- | --- | --- | --- | --- |
44
}
45
46
|     | resource |     | "aws_instance" |     |     | "serveur" | {   |     |
| --- | -------- | --- | -------------- | --- | --- | --------- | --- | --- |
47
|     | count |     |     | = var.instance_count |     |     |     |     |
| --- | ----- | --- | --- | -------------------- | --- | --- | --- | --- |
48
| 49  | ami           |     |     | = data.aws_ami.ubuntu.id |     |     |     |     |
| --- | ------------- | --- | --- | ------------------------ | --- | --- | --- | --- |
|     | instance_type |     |     | = "t3.micro"             |     |     |     |     |
50
|     | subnet_id |     |     | = aws_subnet.public.id |     |     |     |     |
| --- | --------- | --- | --- | ---------------------- | --- | --- | --- | --- |
51
tags = { Name = "serveur-${var.environment}-${count.index}" }
52
53 }
54
# Outputs
55
| 56  | output | "instance_ips" |                                   |     | {   |     |     |     |
| --- | ------ | -------------- | --------------------------------- | --- | --- | --- | --- | --- |
|     | value  | =              | aws_instance.serveur[*].public_ip |     |     |     |     |     |
57
51

| Module |     | DevOps |     |     |     |     |     |     |     | S8-SIIA |
| ------ | --- | ------ | --- | --- | --- | --- | --- | --- | --- | ------- |
}
58
Listing 7.3 – Exemple infrastructure AWS avec Terraform (main.tf)
| 7.3   |     | Ansible      |     |     |     |     |     |     |     |     |
| ----- | --- | ------------ | --- | --- | --- | --- | --- | --- | --- | --- |
| 7.3.1 |     | Présentation |     |     |     |     |     |     |     |     |
Ansible est un outil d’automatisation agentless (sans agent) qui permet de configurer
des systèmes, de déployer des applications et d’orchestrer des tâches complexes. Il utilise
| SSH   | pour     | communiquer  |          | avec | les | machines | cibles. |     |     |     |
| ----- | -------- | ------------ | -------- | ---- | --- | -------- | ------- | --- | --- | --- |
| 7.3.2 |          | Installation |          |      |     |          |         |     |     |     |
| 1     | # Ubuntu |              | / Debian |      |     |          |         |     |     |     |
|       | sudo     | apt-get      | update   |      |     |          |         |     |     |     |
2
|     | sudo | apt-get | install |     | -y  | software-properties-common |     |     |     |     |
| --- | ---- | ------- | ------- | --- | --- | -------------------------- | --- | --- | --- | --- |
3
| 4   | sudo | add-apt-repository |         |     |     | --yes   | --update |     | ppa:ansible/ansible |     |
| --- | ---- | ------------------ | ------- | --- | --- | ------- | -------- | --- | ------------------- | --- |
|     | sudo | apt-get            | install |     | -y  | ansible |          |     |                     |     |
5
6
|     | # Via | pip |     |     |     |     |     |     |     |     |
| --- | ----- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
7
| 8   | pip | install | ansible |     | --break-system-packages |     |     |     |     |     |
| --- | --- | ------- | ------- | --- | ----------------------- | --- | --- | --- | --- | --- |
9
|     | # Verifier |     | l’installation |     |     |     |     |     |     |     |
| --- | ---------- | --- | -------------- | --- | --- | --- | --- | --- | --- | --- |
10
| 11    | ansible  | --version |                 |                |         |        |                |      |           |     |
| ----- | -------- | --------- | --------------- | -------------- | ------- | ------ | -------------- | ---- | --------- | --- |
|       |          |           |                 |                | Listing | 7.4    | – Installation |      | d’Ansible |     |
| 7.3.3 |          | Commandes |                 |                | Ansible |        |                |      |           |     |
| 1     | # Tester |           | la connectivite |                |         | (ping) |                |      |           |     |
|       | ansible  | all       | -i              | inventaire.ini |         |        | -m             | ping |           |     |
2
|     | ansible | webservers |     |     | -i  | inventaire.ini |     |     | -m ping |     |
| --- | ------- | ---------- | --- | --- | --- | -------------- | --- | --- | ------- | --- |
3
4
| 5   | # Executer |     | une | commande       |     | ad-hoc |     |         |             |     |
| --- | ---------- | --- | --- | -------------- | --- | ------ | --- | ------- | ----------- | --- |
|     | ansible    | all | -i  | inventaire.ini |     |        | -m  | command | -a "uptime" |     |
6
|     | ansible | all | -i  | inventaire.ini |     |     | -m  | shell | -a "df | -h" |
| --- | ------- | --- | --- | -------------- | --- | --- | --- | ----- | ------ | --- |
7
| 8   | ansible | webservers  |     |                  | -i  | inventaire.ini |     |          | -m service | \   |
| --- | ------- | ----------- | --- | ---------------- | --- | -------------- | --- | -------- | ---------- | --- |
|     | -a      | "name=nginx |     | state=restarted" |     |                |     | --become |            |     |
9
10
|     | # Copier |     | un fichier |     |     |     |     |     |     |     |
| --- | -------- | --- | ---------- | --- | --- | --- | --- | --- | --- | --- |
11
| 12  | ansible | all               | -i  | inventaire.ini |     |                             | -m  | copy | \   |     |
| --- | ------- | ----------------- | --- | -------------- | --- | --------------------------- | --- | ---- | --- | --- |
|     | -a      | "src=fichier.conf |     |                |     | dest=/etc/app/fichier.conf" |     |      |     |     |
13
14
| 15  | # Installer |     | un  | paquet         |     |     |     |     |     |     |
| --- | ----------- | --- | --- | -------------- | --- | --- | --- | --- | --- | --- |
|     | ansible     | all | -i  | inventaire.ini |     |     | -m  | apt | \   |     |
16
|     | -a  | "name=nginx |     | state=present" |     |     |     | --become |     |     |
| --- | --- | ----------- | --- | -------------- | --- | --- | --- | -------- | --- | --- |
17
18
| 19  | # Executer       |     | un playbook |     |                |     |     |     |              |     |
| --- | ---------------- | --- | ----------- | --- | -------------- | --- | --- | --- | ------------ | --- |
|     | ansible-playbook |     |             | -i  | inventaire.ini |     |     |     | playbook.yml |     |
20
52

| Module DevOps |     |     |     |     |     |     |     | S8-SIIA |
| ------------- | --- | --- | --- | --- | --- | --- | --- | ------- |
21
| 22 # Executer    | en  | mode | dry-run           |     | (check) |              |     |         |
| ---------------- | --- | ---- | ----------------- | --- | ------- | ------------ | --- | ------- |
| ansible-playbook |     |      | -i inventaire.ini |     |         | playbook.yml |     | --check |
23
24
| 25 # Afficher    | les | differences |                   |     |     |              |     |        |
| ---------------- | --- | ----------- | ----------------- | --- | --- | ------------ | --- | ------ |
| ansible-playbook |     |             | -i inventaire.ini |     |     | playbook.yml |     | --diff |
26
27
| # Limiter | l’execution |     |     | a un | groupe |     |     |     |
| --------- | ----------- | --- | --- | ---- | ------ | --- | --- | --- |
28
| 29 ansible-playbook |            |     | -i inventaire.ini |     |     | playbook.yml |     | \   |
| ------------------- | ---------- | --- | ----------------- | --- | --- | ------------ | --- | --- |
| --limit             | webservers |     |                   |     |     |              |     |     |
30
31
| 32 # Passer      | des | variables |                   | extra |     |              |     |     |
| ---------------- | --- | --------- | ----------------- | ----- | --- | ------------ | --- | --- |
| ansible-playbook |     |           | -i inventaire.ini |       |     | playbook.yml |     | \   |
33
| -e "env=production |     |     |     | version=2.0.0" |     |     |     |     |
| ------------------ | --- | --- | --- | -------------- | --- | --- | --- | --- |
34
35
| 36 # Afficher    | les | taches |              | disponibles |              |     |     |     |
| ---------------- | --- | ------ | ------------ | ----------- | ------------ | --- | --- | --- |
| ansible-playbook |     |        | playbook.yml |             | --list-tasks |     |     |     |
37
38
| 39 # Afficher    | les | hotes |              | cibles |              |     |     |     |
| ---------------- | --- | ----- | ------------ | ------ | ------------ | --- | --- | --- |
| ansible-playbook |     |       | playbook.yml |        | --list-hosts |     |     |     |
40
41
| # Executer | avec | plus |     | de  | verbosit |     |     |     |
| ---------- | ---- | ---- | --- | --- | -------- | --- | --- | --- |
42
| ansible-playbook |     |     | -i inventaire.ini |     |     | playbook.yml |     | -v  |
| ---------------- | --- | --- | ----------------- | --- | --- | ------------ | --- | --- |
43
| ansible-playbook |     |     | -i inventaire.ini |     |     | playbook.yml |     | -vvv |
| ---------------- | --- | --- | ----------------- | --- | --- | ------------ | --- | ---- |
44
45
| 46 # Verifier    | la  | syntaxe |              | d’un | playbook       |     |     |     |
| ---------------- | --- | ------- | ------------ | ---- | -------------- | --- | --- | --- |
| ansible-playbook |     |         | playbook.yml |      | --syntax-check |     |     |     |
47
48
| 49 # Gestion   | des | roles | (Galaxy) |     |                   |     |     |     |
| -------------- | --- | ----- | -------- | --- | ----------------- | --- | --- | --- |
| ansible-galaxy |     | role  | install  |     | geerlingguy.nginx |     |     |     |
50
| ansible-galaxy |     | collection |     |     | install | community.docker |     |     |
| -------------- | --- | ---------- | --- | --- | ------- | ---------------- | --- | --- |
51
| ansible-galaxy |     | list |     |     |     |     |     |     |
| -------------- | --- | ---- | --- | --- | --- | --- | --- | --- |
52
53
| # Initialiser |     | un  | nouveau |     | role |     |     |     |
| ------------- | --- | --- | ------- | --- | ---- | --- | --- | --- |
54
| ansible-galaxy |     | role | init |     | mon-role |     |     |     |
| -------------- | --- | ---- | ---- | --- | -------- | --- | --- | --- |
55
56
| # Chiffrer | un  | fichier |     | avec | Vault |     |     |     |
| ---------- | --- | ------- | --- | ---- | ----- | --- | --- | --- |
57
| ansible-vault |     | encrypt |     | secrets.yml |     |     |     |     |
| ------------- | --- | ------- | --- | ----------- | --- | --- | --- | --- |
58
| ansible-vault |     | decrypt |     | secrets.yml |     |     |     |     |
| ------------- | --- | ------- | --- | ----------- | --- | --- | --- | --- |
59
| 60 ansible-vault |     | view | secrets.yml |     |     |     |     |     |
| ---------------- | --- | ---- | ----------- | --- | --- | --- | --- | --- |
| ansible-vault    |     | edit | secrets.yml |     |     |     |     |     |
61
62
| 63 # Executer    | avec | Vault |              |     |                  |     |     |     |
| ---------------- | ---- | ----- | ------------ | --- | ---------------- | --- | --- | --- |
| ansible-playbook |      |       | playbook.yml |     | --ask-vault-pass |     |     |     |
64
| ansible-playbook |     |     | playbook.yml |     | \   |     |     |     |
| ---------------- | --- | --- | ------------ | --- | --- | --- | --- | --- |
65
| --vault-password-file |     |     |     | ~/.vault_pass |     |     |     |     |
| --------------------- | --- | --- | --- | ------------- | --- | --- | --- | --- |
66
|     |     |     | Listing |     | 7.5 – Commandes |     | Ansible |     |
| --- | --- | --- | ------- | --- | --------------- | --- | ------- | --- |
53
