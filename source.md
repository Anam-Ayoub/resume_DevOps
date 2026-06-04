# Chapitre 1 — Introduction et Culture DevOps
 
---
 
## 1.1 Historique et Contexte
 
Le terme **DevOps** est une contraction de *Development* (développement) et *Operations* (exploitation). Il désigne un ensemble de pratiques, de méthodes et d'outils visant à améliorer la collaboration entre les équipes de développement logiciel et les équipes d'exploitation informatique.
 
Avant DevOps, les organisations travaillaient en **silos** : les développeurs écrivaient du code et le transmettaient aux équipes opérationnelles qui se chargeaient de le déployer et de le maintenir en production. Cette approche générait de nombreux problèmes : conflits de responsabilité, délais de mise en production longs, instabilité des systèmes.
 
---
 
## 1.2 Définition et Philosophie
 
> **Définition :** DevOps est une approche culturelle, organisationnelle et technique qui vise à unifier le développement logiciel (Dev) et l'administration des systèmes informatiques (Ops) afin de livrer des applications de manière **continue**, **fiable** et **rapide**.
 
### 1.2.1 Les trois piliers du DevOps
 
1. **Culture** : collaboration, partage de responsabilités, apprentissage continu.
2. **Automatisation** : réduction des tâches manuelles répétitives.
3. **Mesure** : collecte de métriques, amélioration continue basée sur les données.
---
 
## 1.3 Le Cycle de Vie DevOps (CALMS)
 
Le modèle **CALMS** résume les valeurs fondamentales du DevOps :
 
| Lettre | Signification |
|--------|---------------|
| **C**  | Culture (collaboration entre Dev et Ops) |
| **A**  | Automatisation (des processus répétitifs) |
| **L**  | Lean (réduction du gaspillage) |
| **M**  | Measurement (métriques et feedback) |
| **S**  | Sharing (partage des connaissances) |
 
---
 
## 1.4 Le Pipeline DevOps
 
Le cycle de vie DevOps comprend les phases suivantes :
 
1. **Plan** : définition des besoins et des objectifs.
2. **Code** : développement du logiciel.
3. **Build** : compilation et assemblage du code.
4. **Test** : vérification automatique de la qualité.
5. **Release** : préparation du livrable.
6. **Deploy** : déploiement en production.
7. **Operate** : gestion de l'infrastructure en production.
8. **Monitor** : surveillance et collecte de métriques.
---
 
## 1.5 Avantages du DevOps
 
- Réduction du délai de mise sur le marché (*time-to-market*).
- Amélioration de la qualité logicielle.
- Meilleure stabilité des systèmes en production.
- Réduction des coûts opérationnels.
- Augmentation de la satisfaction client.
---

# Chapitre 2 — Gestion de Versions et Collaboration avec Git

---

## 2.1 Introduction à Git

**Git** est un système de gestion de versions *distribué* créé par Linus Torvalds en 2005. Il permet de suivre les modifications du code source, de collaborer efficacement et de gérer plusieurs versions d'un projet simultanément.

> **Dépôt (Repository) :** répertoire versionné contenant l'ensemble du code source et l'historique complet des modifications.

---

## 2.2 Installation et Configuration initiale

**Listing 2.1 – Installation de Git**
```bash
# Debian / Ubuntu
sudo apt-get update && sudo apt-get install -y git

# CentOS / RHEL
sudo yum install -y git

# macOS (avec Homebrew)
brew install git
```

**Listing 2.2 – Configuration globale de Git**
```bash
# Définir le nom d'utilisateur
git config --global user.name "Prenom NOM"

# Définir l'adresse email
git config --global user.email "prenom.nom@exemple.com"

# Définir l'éditeur par défaut
git config --global core.editor vim

# Définir la branche principale par défaut
git config --global init.defaultBranch main

# Afficher la configuration actuelle
git config --list

# Afficher un paramètre spécifique
git config user.name
```

---

## 2.3 Commandes Fondamentales

### 2.3.1 Initialisation et Clonage

**Listing 2.3 – Initialisation et clonage d'un dépôt**
```bash
# Initialiser un nouveau dépôt local
git init

# Initialiser un dépôt avec un nom de répertoire
git init mon-projet

# Cloner un dépôt distant (HTTPS)
git clone https://github.com/utilisateur/depot.git

# Cloner avec SSH
git clone git@github.com:utilisateur/depot.git

# Cloner dans un répertoire spécifique
git clone https://github.com/utilisateur/depot.git mon-dossier

# Cloner une branche spécifique
git clone -b develop https://github.com/utilisateur/depot.git

# Cloner sans l'historique complet (shallow clone)
git clone --depth 1 https://github.com/utilisateur/depot.git
```

---

### 2.3.2 Suivre les Fichiers (Staging)

**Listing 2.4 – Zone de transit (staging area)**
```bash
# Afficher l'état du dépôt
git status

# Afficher l'état en format court
git status -s

# Ajouter un fichier spécifique à la zone de transit
git add fichier.txt

# Ajouter tous les fichiers modifiés
git add .

# Ajouter tous les fichiers d'une extension
git add *.java

# Ajouter de manière interactive (sélectif)
git add -p

# Retirer un fichier de la zone de transit
git restore --staged fichier.txt

# Ancienne syntaxe équivalente
git reset HEAD fichier.txt
```

---

### 2.3.3 Valider les Modifications (Commit)

**Listing 2.5 – Commandes de commit**
```bash
# Créer un commit avec un message
git commit -m "feat: ajout de la fonctionnalité de connexion"

# Ajouter et committer en une seule commande
git commit -am "fix: correction du bug d'authentification"

# Amender le dernier commit (message ou contenu)
git commit --amend -m "feat: nouveau message"

# Amender sans changer le message
git commit --amend --no-edit

# Commit vide (utile pour CI)
git commit --allow-empty -m "trigger CI"
```

---

### 2.3.4 Consulter l'Historique

**Listing 2.6 – Consultation de l'historique**
```bash
# Afficher l'historique des commits
git log

# Afficher l'historique en une ligne par commit
git log --oneline

# Afficher avec graphe des branches
git log --oneline --graph --all

# Afficher les n derniers commits
git log -n 5

# Filtrer par auteur
git log --author="AATTOURI"

# Filtrer par date
git log --since="2024-01-01" --until="2024-12-31"

# Afficher les modifications d'un commit
git show <hash-commit>

# Afficher les différences non committées
git diff

# Afficher les différences entre la zone de transit et le dernier commit
git diff --staged
```

---

### 2.3.5 Gestion des Branches

**Listing 2.7 – Gestion des branches**
```bash
# Lister les branches locales
git branch

# Lister toutes les branches (locales et distantes)
git branch -a

# Créer une nouvelle branche
git branch feature/ma-fonctionnalite

# Basculer sur une branche existante
git checkout develop
git switch develop          # nouvelle syntaxe recommandée

# Créer et basculer sur une nouvelle branche
git checkout -b feature/ma-fonctionnalite
git switch -c feature/ma-fonctionnalite   # nouvelle syntaxe

# Renommer une branche
git branch -m ancien-nom nouveau-nom

# Supprimer une branche locale
git branch -d feature/ma-fonctionnalite

# Forcer la suppression d'une branche non mergée
git branch -D feature/ma-fonctionnalite

# Supprimer une branche distante
git push origin --delete feature/ma-fonctionnalite
```

---

### 2.3.6 Fusion et Rebase

**Listing 2.8 – Fusion de branches**
```bash
# Fusionner une branche dans la branche courante
git merge feature/ma-fonctionnalite

# Fusion sans fast-forward (conserve l'historique)
git merge --no-ff feature/ma-fonctionnalite

# Rebaser la branche courante sur main
git rebase main

# Rebaser interactivement les 3 derniers commits
git rebase -i HEAD~3

# Abandonner un rebase en cours
git rebase --abort

# Continuer après résolution de conflit
git rebase --continue

# Cherry-pick : appliquer un commit spécifique
git cherry-pick <hash-commit>
```

---

### 2.3.7 Interaction avec le Dépôt Distant

**Listing 2.9 – Commandes distantes (remote)**
```bash
# Afficher les dépôts distants
git remote -v

# Ajouter un dépôt distant
git remote add origin https://github.com/utilisateur/depot.git

# Modifier l'URL d'un dépôt distant
git remote set-url origin git@github.com:utilisateur/depot.git

# Supprimer un dépôt distant
git remote remove origin

# Récupérer les modifications sans merger
git fetch origin

# Récupérer toutes les branches distantes
git fetch --all

# Tirer (fetch + merge) la branche courante
git pull

# Tirer avec rebase
git pull --rebase

# Pousser la branche courante vers le dépôt distant
git push origin main

# Pousser et configurer le suivi
git push -u origin feature/ma-fonctionnalite

# Pousser tous les tags
git push --tags
```

---

### 2.3.8 Annuler des Modifications

**Listing 2.10 – Annulation et restauration**
```bash
# Annuler les modifications d'un fichier (non staged)
git restore fichier.txt

# Réinitialiser la zone de transit
git restore --staged fichier.txt

# Revenir à un commit précédent (soft : conserve les modifications)
git reset --soft HEAD~1

# Revenir à un commit précédent (mixed : défaut)
git reset HEAD~1

# Revenir à un commit précédent (hard : perd les modifications)
git reset --hard HEAD~1

# Créer un commit annulant un commit précédent
git revert <hash-commit>

# Mettre de côté des modifications temporairement
git stash

# Mettre de côté avec un nom
git stash push -m "travail en cours sur feature X"

# Lister les stash
git stash list

# Appliquer le dernier stash
git stash apply

# Appliquer un stash spécifique
git stash apply stash@{2}

# Appliquer et supprimer le dernier stash
git stash pop

# Supprimer un stash
git stash drop stash@{0}

# Supprimer tous les stash
git stash clear
```

---

### 2.3.9 Étiquettes (Tags)

**Listing 2.11 – Gestion des tags**
```bash
# Créer un tag léger
git tag v1.0.0

# Créer un tag annoté (recommandé)
git tag -a v1.0.0 -m "Version 1.0.0 stable"

# Tagger un commit spécifique
git tag -a v0.9.0 <hash-commit>

# Lister les tags
git tag

# Afficher les détails d'un tag
git show v1.0.0

# Pousser un tag spécifique
git push origin v1.0.0

# Pousser tous les tags
git push origin --tags

# Supprimer un tag local
git tag -d v1.0.0

# Supprimer un tag distant
git push origin --delete v1.0.0
```

---

## 2.4 Stratégies de Branchement

### 2.4.1 Git Flow

Git Flow est une stratégie de branchement populaire définissant un modèle strict de branches :

| Branche       | Rôle                                          |
|---------------|-----------------------------------------------|
| `main`        | Code de production stable                     |
| `develop`     | Branche d'intégration principale              |
| `feature/*`   | Nouvelles fonctionnalités                     |
| `release/*`   | Préparation à la mise en production           |
| `hotfix/*`    | Corrections urgentes en production            |

**Listing 2.12 – Git Flow avec l'outil git-flow**
```bash
# Installer git-flow
sudo apt-get install git-flow

# Initialiser git-flow dans un dépôt existant
git flow init

# Démarrer une nouvelle fonctionnalité
git flow feature start ma-fonctionnalite

# Terminer une fonctionnalité
git flow feature finish ma-fonctionnalite

# Démarrer une release
git flow release start 1.2.0

# Terminer une release
git flow release finish 1.2.0

# Démarrer un hotfix
git flow hotfix start correction-critique

# Terminer un hotfix
git flow hotfix finish correction-critique
```

---

### 2.4.2 Trunk-Based Development

Dans cette approche, tous les développeurs committent directement sur une branche unique (`main` ou `trunk`). Les fonctionnalités non finies sont masquées par des **feature flags**.

---

## 2.5 Fichier .gitignore

Le fichier `.gitignore` liste les fichiers et répertoires que Git doit ignorer (fichiers de compilation, secrets, dépendances, fichiers d'IDE, etc.).

**Listing 2.13 – Exemple de fichier .gitignore**
```gitignore
# Fichiers de compilation Java
*.class
*.jar
target/

# Environnements virtuels Python
venv/
__pycache__/
*.pyc

# Variables d'environnement
.env
.env.local

# Fichiers de l'IDE
.idea/
.vscode/
*.swp

# Système d'exploitation
.DS_Store
Thumbs.db

# Dépendances Node.js
node_modules/
npm-debug.log
```

```bash
# Vérifier quels fichiers seront ignorés
git check-ignore -v fichier.txt

# Forcer l'ajout d'un fichier ignoré
git add -f fichier.log
```

---

# Chapitre 3 : Intégration Continue (CI)

## 3.1 Définition et Principes

> L'**Intégration Continue** (*Continuous Integration* ou **CI**) est une pratique de développement logicielle qui consiste à intégrer fréquemment les modifications de code au sein d'un dépôt partagé unique. Chaque intégration déclenche automatiquement une suite de *builds* et de tests afin de détecter et de corriger au plus tôt les régressions.

La mise en œuvre de la **CI** repose sur huit principes fondamentaux décrits dans le tableau suivant :

| N° | Principes fondamentaux de l'Intégration Continue |
| :---: | :--- |
| **1** | Maintenir un dépôt de code unique et partagé. |
| **2** | Automatiser la phase de construction (*build*). |
| **3** | Rendre la construction auto-testable. |
| **4** | Intégrer quotidiennement les modifications de code. |
| **5** | Assurer un *build* rapide (durée inférieure à 10 minutes). |
| **6** | Exécuter les tests dans un environnement identique à la production. |
| **7** | Assurer la transparence en rendant les résultats accessibles à tous. |
| **8** | Automatiser le processus de déploiement. |

---

## 3.2 Jenkins

### 3.2.1 Présentation

> **Jenkins** est un serveur d'automatisation *open-source* développé en *Java*, s'imposant comme le standard incontournable pour concevoir des pipelines **CI/CD**. Son immense écosystème de *plugins* lui permet de s'interfacer nativement avec des technologies clés telles que **Git**, **Docker**, **Kubernetes** ou encore **Slack**.

### 3.2.2 Installation de Jenkins
### Installation de Jenkins sur Ubuntu
```bash
# Installer Java (prerequis)
sudo apt-get update
sudo apt-get install -y openjdk-17-jdk

# Ajouter la cle GPG de Jenkins
curl -fsSL [https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key](https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key) \
sudo tee /usr/share/keyrings/jenkins-keyring.asc > /dev/null

# Ajouter le depot Jenkins
echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
[https://pkg.jenkins.io/debian-stable](https://pkg.jenkins.io/debian-stable) binary/" \
sudo tee /etc/apt/sources.list.d/jenkins.list > /dev/null

# Installer Jenkins
sudo apt-get update
sudo apt-get install -y jenkins

# Demarrer et activer Jenkins
sudo systemctl start jenkins
sudo systemctl enable jenkins

# Verifier le statut
sudo systemctl status jenkins

# Recuperer le mot de passe initial
sudo cat /var/lib/jenkins/secrets/initialAdminPassword
```
### Installation de Jenkins via Docker

```bash
# Lancer Jenkins dans un conteneur Docker
docker run -d \
--name jenkins \
-p 8080:8080 \
-p 50000:50000 \
-v jenkins_home:/var/jenkins_home \
jenkins/jenkins:lts-jdk17

# Recuperer le mot de passe initial
docker exec jenkins cat /var/jenkins_home/secrets/initialAdminPassword
```

### 3.2.3 Gestion de Jenkins via CLI
### Jenkins CLI
```bash
# Telecharger le client CLI
wget http://localhost:8080/jnlpJars/jenkins-cli.jar

# Se connecter au serveur Jenkins
java -jar jenkins-cli.jar \
-s http://localhost:8080 \
-auth admin:mon-mot-de-passe \
help

# Lister les jobs
java -jar jenkins-cli.jar \
-s http://localhost:8080 \
-auth admin:token \
list-jobs

# Declencher un build
java -jar jenkins-cli.jar \
-s http://localhost:8080 \
-auth admin:token \
build mon-job

# Activer/desactiver un job
java -jar jenkins-cli.jar -s http://localhost:8080 -auth admin:token disable-job mon-job
java -jar jenkins-cli.jar -s http://localhost:8080 -auth admin:token enable-job mon-job

# Supprimer un job
java -jar jenkins-cli.jar -s http://localhost:8080 -auth admin:token delete-job mon-job

# Installer un plugin
java -jar jenkins-cli.jar -s http://localhost:8080 -auth admin:token install-plugin git

# Recharger la configuration
java -jar jenkins-cli.jar -s http://localhost:8080 -auth admin:token reload-configuration

# Redemarrer Jenkins
java -jar jenkins-cli.jar -s http://localhost:8080 -auth admin:token restart
```

### 3.2.4 Jenkinsfile – Pipeline Déclaratif
Le Jenkinsfile est un fichier textuel positionné à la racine du dépôt de code. Il concrétise l'approche de Pipeline as Code en décrivant l'intégralité du processus de livraison.

### Structure d’un Jenkinsfile declaratif

```Groovy
pipeline {
    agent any

    environment {
        MAVEN_HOME = tool 'Maven-3.9'
        APP_VERSION = '1.0.0'
        DOCKER_IMAGE = "monapp:${APP_VERSION}"
    }

    options {
        timeout(time: 30, unit: 'MINUTES')
        disableConcurrentBuilds()
        buildDiscarder(logRotator(numToKeepStr: '10'))
    }

    triggers {
        pollSCM('H/5 * * * *') // Toutes les 5 minutes
        cron('H 2 * * 1-5') // Chaque nuit en semaine
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: '[https://github.com/utilisateur/depot.git](https://github.com/utilisateur/depot.git)'
            }
        }

        stage('Build') {
            steps {
                sh "${MAVEN_HOME}/bin/mvn clean package -DskipTests"
            }
        }

        stage('Tests Unitaires') {
            steps {
                sh "${MAVEN_HOME}/bin/mvn test"
            }
            post {
                always {
                    junit '**/target/surefire-reports/*.xml'
                }
            }
        }

        stage('Analyse Qualite') {
            steps {
                withSonarQubeEnv('SonarQube') {
                    sh "${MAVEN_HOME}/bin/mvn sonar:sonar"
                }
            }
        }

        stage('Quality Gate') {
            steps {
                timeout(time: 5, unit: 'MINUTES') {
                    waitForQualityGate abortPipeline: true
                }
            }
        }

        stage('Build Docker') {
            steps {
                sh "docker build -t ${DOCKER_IMAGE} ."
            }
        }

        stage('Push Image') {
            steps {
                withCredentials([usernamePassword(
                    credentialsId: 'docker-hub',
                    usernameVariable: 'DOCKER_USER',
                    passwordVariable: 'DOCKER_PASS'
                )]) {
                    sh """
                    echo ${DOCKER_PASS} docker login -u ${DOCKER_USER} --password-stdin
                    docker push ${DOCKER_IMAGE}
                    """
                }
            }
        }

        stage('Deploiement Staging') {
            when {
                branch 'develop'
            }
            steps {
                sh "kubectl apply -f k8s/staging/"
            }
        }

        stage('Deploiement Production') {
            when {
                branch 'main'
            }
            input {
                message "Deployer en production ?"
                ok "Deployer"
            }
            steps {
                sh "kubectl apply -f k8s/production/"
            }
        }
    }

    post {
        success {
            slackSend channel: '#devops', message: "Build REUSSI : ${env.JOB_NAME} #${env.BUILD_NUMBER}"
        }
        failure {
            emailext to: 'equipe@exemple.com', subject: "ECHEC : ${env.JOB_NAME} #${env.BUILD_NUMBER}", body: "Verifiez les logs : ${env.BUILD_URL}"
        }
        always {
            cleanWs()
        }
    }
}
```
### Pipeline Scripted (Groovy)
```Groovy
node('linux') {
    def mavenHome = tool 'Maven-3.9'

    stage('Checkout') {
        checkout scm
    }

    stage('Build') {
        try {
            sh "${mavenHome}/bin/mvn clean package"
        } catch (Exception e) {
            currentBuild.result = 'FAILURE'
            error "Le build a echoue : ${e.message}"
        }
    }

    stage('Deploiement') {
        if (env.BRANCH_NAME == 'main') {
            sh 'kubectl apply -f k8s/'
        }
    }
}
```

### 3.2.5 Gestion des Credentials Jenkins
L'utilisation des différents types de secrets (credentials) gérés de manière sécurisée par Jenkins s'articule comme suit :

Type de Secret,Description et Syntaxe Contextuelle
Username / Password,Injecte séparément un nom d'utilisateur et un mot de passe sous forme de variables.
Secret Text,Utilisé généralement pour stocker un jeton d'API (API token) ou une clé de sécurité brute.
Fichier Secret,Permet de manipuler un fichier confidentiel (ex: configuration kubeconfig) via son chemin local temporaire.
SSH Private Key,Injecte une clé privée SSH et un identifiant utilisateur associé pour s'authentifier à distance.

| Type de Secret        | Description et Syntaxe Contextuelle                                                                        |
|-----------------------|------------------------------------------------------------------------------------------------------------|
| `Username / Password` | Injecte séparément un nom d'utilisateur et un mot de passe sous forme de variables                         |
| `Secret Text`         | Utilisé généralement pour stocker un jeton d'API (API token) ou une clé de sécurité brute                  |
| `Fichier Secret`      | Permet de manipuler un fichier confidentiel (ex: configuration kubeconfig) via son chemin local temporaire |
| `SSH Private Key`     | Injecte une clé privée SSH et un identifiant utilisateur associé pour s'authentifier à distance            |

### Utilisation des credentials dans Jenkins
```Groovy
// Credential de type Username/Password
withCredentials([usernamePassword(
    credentialsId: 'mon-credential-id',
    usernameVariable: 'USER',
    passwordVariable: 'PASS'
)]) {
    sh "curl -u ${USER}:${PASS} [https://api.exemple.com](https://api.exemple.com)"
}

// Credential de type Secret Text
withCredentials([string(credentialsId: 'api-token', variable: 'TOKEN')]) {
    sh "curl -H 'Authorization: Bearer ${TOKEN}' [https://api.exemple.com](https://api.exemple.com)"
}

// Credential de type Fichier Secret
withCredentials([file(credentialsId: 'kubeconfig', variable: 'KUBECONFIG')]) {
    sh "kubectl --kubeconfig=${KUBECONFIG} get pods"
}

// Credential de type SSH
withCredentials([sshUserPrivateKey(
    credentialsId: 'ssh-key',
    keyFileVariable: 'SSH_KEY',
    usernameVariable: 'SSH_USER'
)]) {
    sh "ssh -i ${SSH_KEY} ${SSH_USER}@serveur.exemple.com 'date'"
}
```

### 3.2.6 GitHub Actions – Alternative à Jenkins
GitHub Actions est une alternative native à Jenkins intégrée à l'écosystème GitHub. Elle s'appuie sur une description declarative au format YAML pour automatiser les workflows de livraison logicielle.

### Workflow GitHub Actions (.github/workflows/ci.yml)
```YAML
name: Pipeline CI/CD

on:
  push:
    branches: [main, develop]
  pull_request:
    branches: [main]

env:
  DOCKER_IMAGE: monapp

jobs:
  build-and-test:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout du code
        uses: actions/checkout@v4

      - name: Configuration de Java 17
        uses: actions/setup-java@v4
        with:
          java-version: '17'
          distribution: 'temurin'

      - name: Cache Maven
        uses: actions/cache@v3
        with:
          path: ~/.m2
          key: ${{ runner.os }}-m2-${{ hashFiles('**/pom.xml') }}

      - name: Build et tests
        run: mvn clean verify

      - name: Publication des resultats de tests
        uses: actions/upload-artifact@v4
        with:
          name: test-results
          path: target/surefire-reports/

  docker:
    needs: build-and-test
    runs-on: ubuntu-latest
    if: github.ref == 'refs/heads/main'
    steps:
      - uses: actions/checkout@v4

      - name: Login Docker Hub
        uses: docker/login-action@v3
        with:
          username: ${{ secrets.DOCKER_USERNAME }}
          password: ${{ secrets.DOCKER_PASSWORD }}

      - name: Build et Push de l'image
        uses: docker/build-push-action@v5
        with:
          push: true
          tags: ${{ secrets.DOCKER_USERNAME }}/${{ env.DOCKER_IMAGE }}:latest
```

---

# Chapitre 4 — Livraison et Déploiement Continu (CD)

---

## 4.1 Définitions

> **Livraison Continue (Continuous Delivery) :** extension de la CI qui garantit que le code peut être déployé en production à tout moment, après **validation manuelle**.

> **Déploiement Continu (Continuous Deployment) :** extension de la livraison continue où chaque modification validée par les tests est **automatiquement** déployée en production, sans intervention humaine.

---

## 4.2 Stratégies de Déploiement

### 4.2.1 Blue-Green Deployment

Deux environnements identiques coexistent (**Blue** = actuel, **Green** = nouveau). Le trafic est basculé vers Green une fois les tests validés. En cas de problème, le retour arrière est immédiat.

### 4.2.2 Canary Deployment

La nouvelle version est déployée **progressivement** : d'abord pour 5 % des utilisateurs, puis 25 %, puis 100 %. Permet de détecter les régressions avant un impact total.

### 4.2.3 Rolling Update

Les instances de l'application sont mises à jour progressivement, une par une ou par groupes, **sans interruption de service**.

### 4.2.4 Feature Flags

Les nouvelles fonctionnalités sont déployées dans le code mais masquées par des **indicateurs configurables**, permettant une activation progressive sans nouveau déploiement.

---

# Chapitre 5 — Conteneurisation avec Docker

---

## 5.1 Introduction

> **Conteneur :** unité d'exécution légère et isolée qui regroupe une application et toutes ses dépendances (bibliothèques, configuration, code) dans un environnement standardisé et portable.

**Docker** est la plateforme de conteneurisation la plus utilisée. Elle repose sur les fonctionnalités du noyau Linux : *namespaces* (isolation) et *cgroups* (limitation des ressources).

---

## 5.2 Installation de Docker

**Listing 5.1 – Installation de Docker sur Ubuntu**
```bash
# Supprimer les anciennes versions
sudo apt-get remove -y docker docker-engine docker.io containerd runc

# Installer les dépendances
sudo apt-get update
sudo apt-get install -y \
    ca-certificates \
    curl \
    gnupg \
    lsb-release

# Ajouter la clé GPG officielle de Docker
sudo mkdir -p /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | \
    sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg

# Ajouter le dépôt Docker
echo \
    "deb [arch=$(dpkg --print-architecture) \
    signed-by=/etc/apt/keyrings/docker.gpg] \
    https://download.docker.com/linux/ubuntu \
    $(lsb_release -cs) stable" | \
    sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

# Installer Docker Engine
sudo apt-get update
sudo apt-get install -y \
    docker-ce \
    docker-ce-cli \
    containerd.io \
    docker-buildx-plugin \
    docker-compose-plugin

# Démarrer Docker
sudo systemctl start docker
sudo systemctl enable docker

# Vérifier l'installation
docker version
docker info

# Ajouter l'utilisateur au groupe docker (éviter sudo)
sudo usermod -aG docker $USER
newgrp docker
```

---

## 5.3 Gestion des Images

**Listing 5.2 – Commandes de gestion des images Docker**
```bash
# Rechercher une image sur Docker Hub
docker search ubuntu

# Télécharger une image
docker pull ubuntu:22.04
docker pull nginx:latest
docker pull python:3.11-slim

# Lister les images locales
docker images
docker image ls

# Lister toutes les images (inclus les intermédiaires)
docker image ls -a

# Afficher les détails d'une image
docker image inspect ubuntu:22.04

# Afficher l'historique d'une image
docker image history ubuntu:22.04

# Supprimer une image
docker image rm ubuntu:22.04
docker rmi ubuntu:22.04

# Supprimer les images non utilisées
docker image prune

# Supprimer toutes les images non utilisées (y compris taguées)
docker image prune -a

# Taguer une image
docker tag monapp:latest mon-registry.exemple.com/monapp:v1.0.0

# Pousser une image vers un registre
docker push mon-registry.exemple.com/monapp:v1.0.0

# Sauvegarder une image dans un fichier tar
docker save -o monapp.tar monapp:latest

# Charger une image depuis un fichier tar
docker load -i monapp.tar

# Exporter le système de fichiers d'un conteneur
docker export mon-conteneur -o conteneur.tar

# Importer comme image
docker import conteneur.tar mon-image:importee
```

---

## 5.4 Gestion des Conteneurs

**Listing 5.3 – Commandes de gestion des conteneurs**
```bash
# Créer et démarrer un conteneur
docker run ubuntu:22.04

# Démarrer un conteneur en mode interactif
docker run -it ubuntu:22.04 /bin/bash

# Démarrer en arrière-plan (detached)
docker run -d --name mon-nginx nginx:latest

# Démarrer avec mappage de ports
docker run -d -p 8080:80 --name mon-nginx nginx:latest

# Démarrer avec variables d'environnement
docker run -d \
    -e MYSQL_ROOT_PASSWORD=secret \
    -e MYSQL_DATABASE=mabase \
    --name mon-mysql \
    mysql:8.0

# Démarrer avec volume monté
docker run -d \
    -v /chemin/hote:/chemin/conteneur \
    --name mon-app \
    monapp:latest

# Démarrer avec limites de ressources
docker run -d \
    --memory="512m" \
    --cpus="1.5" \
    --name mon-app \
    monapp:latest

# Démarrer avec politique de redémarrage
docker run -d \
    --restart unless-stopped \
    --name mon-app \
    monapp:latest

# Lister les conteneurs en cours d'exécution
docker ps
docker container ls

# Lister tous les conteneurs (arrêtés inclus)
docker ps -a

# Afficher les statistiques en temps réel
docker stats

# Afficher les statistiques d'un seul conteneur
docker stats mon-nginx

# Inspecter un conteneur
docker inspect mon-nginx

# Afficher les logs d'un conteneur
docker logs mon-nginx

# Suivre les logs en temps réel
docker logs -f mon-nginx

# Afficher les 100 dernières lignes
docker logs --tail 100 mon-nginx

# Exécuter une commande dans un conteneur en cours d'exécution
docker exec -it mon-nginx /bin/bash
docker exec mon-nginx ls /var/www/html

# Copier des fichiers entre l'hôte et un conteneur
docker cp fichier.txt mon-nginx:/var/www/html/
docker cp mon-nginx:/var/log/nginx/access.log .

# Arrêter un conteneur (SIGTERM, puis SIGKILL après 10s)
docker stop mon-nginx

# Forcer l'arrêt immédiatement (SIGKILL)
docker kill mon-nginx

# Démarrer un conteneur arrêté
docker start mon-nginx

# Redémarrer un conteneur
docker restart mon-nginx

# Mettre en pause / reprendre
docker pause mon-nginx
docker unpause mon-nginx

# Supprimer un conteneur (il doit être arrêté)
docker rm mon-nginx

# Supprimer un conteneur en cours d'exécution
docker rm -f mon-nginx

# Supprimer tous les conteneurs arrêtés
docker container prune

# Renommer un conteneur
docker rename mon-nginx nouveau-nom

# Afficher les ports exposés
docker port mon-nginx

# Afficher les processus dans un conteneur
docker top mon-nginx

# Attendre qu'un conteneur s'arrête
docker wait mon-nginx
```

---

## 5.5 Le Dockerfile

**Listing 5.4 – Instructions du Dockerfile**
```dockerfile
# FROM : image de base
FROM ubuntu:22.04
FROM python:3.11-slim AS base

# LABEL : métadonnées de l'image
LABEL maintainer="aattouri@exemple.com"
LABEL version="1.0"
LABEL description="Application DevOps"

# ARG : argument de build (disponible uniquement pendant le build)
ARG APP_VERSION=1.0.0
ARG BUILD_DATE

# ENV : variable d'environnement (disponible à l'exécution)
ENV APP_HOME=/app
ENV APP_VERSION=${APP_VERSION}
ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1

# WORKDIR : répertoire de travail
WORKDIR /app

# RUN : exécuter une commande pendant le build
RUN apt-get update \
    && apt-get install -y --no-install-recommends \
        curl \
        wget \
    && rm -rf /var/lib/apt/lists/*

# COPY : copier des fichiers de l'hôte vers l'image
COPY requirements.txt .
COPY src/ ./src/

# ADD : comme COPY mais supporte URL et .tar.gz (déconseillé sauf besoin spécifique)
ADD https://exemple.com/fichier.tar.gz /tmp/

# RUN pour installer les dépendances Python
RUN pip install --no-cache-dir -r requirements.txt

# USER : changer l'utilisateur courant
RUN adduser --system --group appuser
USER appuser

# EXPOSE : documenter le port exposé (ne publie pas)
EXPOSE 8080

# VOLUME : créer un point de montage
VOLUME ["/app/data", "/app/logs"]

# HEALTHCHECK : vérifier la santé du conteneur
HEALTHCHECK --interval=30s --timeout=10s --start-period=5s --retries=3 \
    CMD curl -f http://localhost:8080/health || exit 1

# ENTRYPOINT : commande principale (non surchargeable sans --entrypoint)
ENTRYPOINT ["python", "-m", "gunicorn"]

# CMD : arguments par défaut de ENTRYPOINT (surchargeable)
CMD ["--bind", "0.0.0.0:8080", "app:application"]
```

**Listing 5.5 – Multi-stage Build (bonne pratique)**
```dockerfile
# Stage 1 : Build
FROM maven:3.9-openjdk-17 AS builder
WORKDIR /build
COPY pom.xml .
COPY src ./src
RUN mvn clean package -DskipTests

# Stage 2 : Production (image finale légère)
FROM openjdk:17-jre-slim AS production
WORKDIR /app

# Créer un utilisateur non-root
RUN addgroup --system --gid 1001 appgroup \
    && adduser --system --uid 1001 --gid 1001 appuser

# Copier uniquement le JAR depuis le stage de build
COPY --from=builder /build/target/monapp.jar app.jar

USER appuser
EXPOSE 8080

HEALTHCHECK --interval=30s --timeout=5s \
    CMD wget -qO- http://localhost:8080/actuator/health || exit 1

ENTRYPOINT ["java", "-jar", "/app/app.jar"]
```

### 5.5.1 Construction d'Images

**Listing 5.6 – Commandes de build Docker**
```bash
# Construire une image depuis le Dockerfile courant
docker build -t monapp:latest .

# Spécifier un Dockerfile alternatif
docker build -f Dockerfile.prod -t monapp:prod .

# Passer des arguments de build
docker build \
    --build-arg APP_VERSION=2.0.0 \
    --build-arg BUILD_DATE=$(date -u +"%Y-%m-%dT%H:%M:%SZ") \
    -t monapp:2.0.0 .

# Construire sans cache
docker build --no-cache -t monapp:latest .

# Spécifier la plateforme cible
docker build --platform linux/amd64 -t monapp:latest .

# Build multi-plateforme avec BuildKit
docker buildx build \
    --platform linux/amd64,linux/arm64 \
    -t monapp:latest \
    --push .

# Afficher les étapes de build
docker build --progress=plain -t monapp:latest .

# Cibler un stage spécifique (multi-stage)
docker build --target builder -t monapp:build .
```

---

## 5.6 Réseaux Docker

**Listing 5.7 – Gestion des réseaux Docker**
```bash
# Lister les réseaux
docker network ls

# Inspecter un réseau
docker network inspect bridge

# Créer un réseau personnalisé
docker network create mon-reseau

# Créer un réseau avec sous-réseau spécifique
docker network create \
    --driver bridge \
    --subnet 192.168.10.0/24 \
    --gateway 192.168.10.1 \
    mon-reseau-custom

# Connecter un conteneur à un réseau
docker network connect mon-reseau mon-conteneur

# Déconnecter un conteneur d'un réseau
docker network disconnect mon-reseau mon-conteneur

# Supprimer un réseau
docker network rm mon-reseau

# Supprimer tous les réseaux non utilisés
docker network prune

# Démarrer un conteneur sur un réseau spécifique
docker run -d \
    --network mon-reseau \
    --name mon-app \
    monapp:latest
```

---

## 5.7 Volumes Docker

**Listing 5.8 – Gestion des volumes Docker**
```bash
# Lister les volumes
docker volume ls

# Créer un volume nommé
docker volume create mes-donnees

# Inspecter un volume
docker volume inspect mes-donnees

# Supprimer un volume
docker volume rm mes-donnees

# Supprimer les volumes non utilisés
docker volume prune

# Monter un volume nommé
docker run -d \
    -v mes-donnees:/var/lib/mysql \
    --name mon-mysql \
    mysql:8.0

# Monter un répertoire de l'hôte (bind mount)
docker run -d \
    -v /home/user/data:/app/data \
    --name mon-app \
    monapp:latest

# Monter en lecture seule
docker run -d \
    -v /home/user/config:/app/config:ro \
    --name mon-app \
    monapp:latest

# Volume temporaire en mémoire (tmpfs)
docker run -d \
    --tmpfs /app/temp:size=100m \
    --name mon-app \
    monapp:latest
```

---

## 5.8 Docker Compose

Docker Compose permet de définir et de gérer des **applications multi-conteneurs** via un fichier de configuration déclaratif.

**Listing 5.9 – Exemple complet de docker-compose.yml**
```yaml
version: '3.9'

networks:
  frontend:
    driver: bridge
  backend:
    driver: bridge
    internal: true

volumes:
  db-data:
  redis-data:
  app-logs:

services:

  # Service base de données
  db:
    image: postgres:15-alpine
    container_name: postgres
    restart: unless-stopped
    environment:
      POSTGRES_DB: mabase
      POSTGRES_USER: ${DB_USER:-admin}
      POSTGRES_PASSWORD: ${DB_PASSWORD:?DB_PASSWORD requis}
    volumes:
      - db-data:/var/lib/postgresql/data
      - ./init.sql:/docker-entrypoint-initdb.d/init.sql:ro
    networks:
      - backend
    healthcheck:
      test: ["CMD-SHELL", "pg_isready -U $${POSTGRES_USER}"]
      interval: 10s
      timeout: 5s
      retries: 5

  # Service cache
  redis:
    image: redis:7-alpine
    container_name: redis
    restart: unless-stopped
    command: redis-server --requirepass ${REDIS_PASSWORD}
    volumes:
      - redis-data:/data
    networks:
      - backend
    healthcheck:
      test: ["CMD", "redis-cli", "ping"]
      interval: 10s

  # Service application
  app:
    build:
      context: .
      dockerfile: Dockerfile
      args:
        APP_VERSION: ${APP_VERSION:-1.0.0}
    image: monapp:${APP_VERSION:-latest}
    container_name: mon-app
    restart: unless-stopped
    environment:
      DATABASE_URL: postgresql://admin:${DB_PASSWORD}@db:5432/mabase
      REDIS_URL: redis://:${REDIS_PASSWORD}@redis:6379
    volumes:
      - app-logs:/app/logs
    ports:
      - "8080:8080"
    depends_on:
      db:
        condition: service_healthy
      redis:
        condition: service_healthy
    networks:
      - frontend
      - backend
    deploy:
      resources:
        limits:
          cpus: '1'
          memory: 512M

  # Service proxy inverse
  nginx:
    image: nginx:alpine
    container_name: nginx
    restart: unless-stopped
    ports:
      - "80:80"
      - "443:443"
    volumes:
      - ./nginx/nginx.conf:/etc/nginx/nginx.conf:ro
      - ./nginx/ssl:/etc/nginx/ssl:ro
    depends_on:
      - app
    networks:
      - frontend
```

**Listing 5.10 – Commandes Docker Compose**
```bash
# Démarrer tous les services (arrière-plan)
docker compose up -d

# Démarrer en reconstruisant les images
docker compose up -d --build

# Démarrer un service spécifique
docker compose up -d app

# Arrêter tous les services
docker compose down

# Arrêter et supprimer les volumes
docker compose down -v

# Lister les conteneurs du projet
docker compose ps

# Afficher les logs de tous les services
docker compose logs

# Suivre les logs d'un service spécifique
docker compose logs -f app

# Exécuter une commande dans un service
docker compose exec app /bin/bash
docker compose exec db psql -U admin -d mabase

# Mettre à l'échelle un service
docker compose scale app=3

# Afficher les processus
docker compose top

# Afficher la configuration fusionnée
docker compose config

# Valider le fichier compose
docker compose config --quiet

# Redémarrer un service spécifique
docker compose restart app

# Reconstruire les images sans démarrer
docker compose build

# Tirer les dernières images
docker compose pull

# Supprimer les conteneurs arrêtés
docker compose rm

# Afficher les différentes versions de la configuration
docker compose -f docker-compose.yml \
    -f docker-compose.override.yml \
    config
```

---

# Chapitre 6 — Orchestration avec Kubernetes

---

## 6.1 Introduction

> **Kubernetes (K8s) :** système d'orchestration de conteneurs open-source développé par Google. Il automatise le déploiement, la mise à l'échelle, la gestion de la haute disponibilité et les mises à jour des applications conteneurisées.

---

## 6.2 Architecture de Kubernetes

### 6.2.1 Composants du Plan de Contrôle (Control Plane)

| Composant | Rôle |
|-----------|------|
| `kube-apiserver` | Point d'entrée de toutes les requêtes API |
| `etcd` | Base de données clé-valeur stockant l'état du cluster |
| `kube-scheduler` | Affecte les Pods aux nœuds workers |
| `kube-controller-manager` | Gère les boucles de contrôle (ReplicaSet, etc.) |
| `cloud-controller-manager` | Interface avec le fournisseur cloud |

### 6.2.2 Composants des Nœuds Workers

| Composant | Rôle |
|-----------|------|
| `kubelet` | Agent qui s'assure que les conteneurs s'exécutent dans un Pod |
| `kube-proxy` | Maintient les règles réseau sur les nœuds |
| `Container Runtime` | Docker, containerd ou CRI-O |

---

## 6.3 Installation et Configuration (kubectl)

**Listing 6.1 – Installation de kubectl**
```bash
# Linux
curl -LO "https://dl.k8s.io/release/$(curl -L -s \
    https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl

# Vérifier l'installation
kubectl version --client

# Configurer la complétion bash
echo 'source <(kubectl completion bash)' >> ~/.bashrc
source ~/.bashrc

# Alias recommandés
alias k='kubectl'
alias kgp='kubectl get pods'
alias kgs='kubectl get services'
alias kgd='kubectl get deployments'
```

**Listing 6.2 – Gestion de la configuration (kubeconfig)**
```bash
# Afficher la configuration courante
kubectl config view

# Afficher le contexte actif
kubectl config current-context

# Lister les contextes disponibles
kubectl config get-contexts

# Changer de contexte
kubectl config use-context mon-cluster-prod

# Définir le namespace par défaut pour un contexte
kubectl config set-context --current --namespace=mon-namespace

# Fusionner plusieurs kubeconfig
KUBECONFIG=~/.kube/config:~/.kube/config-prod \
    kubectl config view --flatten > ~/.kube/config-merge
```

---

## 6.4 Ressources Fondamentales

### 6.4.1 Namespace

**Listing 6.3 – Gestion des Namespaces**
```bash
# Lister les namespaces
kubectl get namespaces
kubectl get ns

# Créer un namespace
kubectl create namespace dev
kubectl create namespace staging
kubectl create namespace production

# Supprimer un namespace (et toutes ses ressources)
kubectl delete namespace dev

# Déployer dans un namespace spécifique
kubectl apply -f deployment.yaml -n staging

# Travailler dans un namespace spécifique
kubectl -n staging get pods
```

---

### 6.4.2 Pod

**Listing 6.4 – Manifeste d'un Pod**
```yaml
apiVersion: v1
kind: Pod
metadata:
  name: mon-pod
  namespace: default
  labels:
    app: monapp
    version: "1.0"
spec:
  containers:
  - name: monapp
    image: monapp:1.0.0
    ports:
    - containerPort: 8080
    env:
    - name: APP_ENV
      value: "production"
    - name: DB_PASSWORD
      valueFrom:
        secretKeyRef:
          name: db-secret
          key: password
    resources:
      requests:
        memory: "128Mi"
        cpu: "250m"
      limits:
        memory: "512Mi"
        cpu: "1000m"
    livenessProbe:
      httpGet:
        path: /health
        port: 8080
      initialDelaySeconds: 30
      periodSeconds: 10
    readinessProbe:
      httpGet:
        path: /ready
        port: 8080
      initialDelaySeconds: 5
      periodSeconds: 5
  restartPolicy: Always
```

**Listing 6.5 – Commandes de gestion des Pods**
```bash
# Lister les pods dans le namespace courant
kubectl get pods
kubectl get pods -o wide           # avec IP et nœud
kubectl get pods --all-namespaces  # tous les namespaces
kubectl get pods -n mon-namespace

# Créer un pod à partir d'un manifeste
kubectl apply -f pod.yaml

# Décrire un pod (événements, configuration)
kubectl describe pod mon-pod

# Afficher les logs d'un pod
kubectl logs mon-pod

# Logs d'un conteneur spécifique dans un pod multi-conteneurs
kubectl logs mon-pod -c nom-conteneur

# Suivre les logs en temps réel
kubectl logs -f mon-pod

# Logs des 100 dernières lignes
kubectl logs --tail=100 mon-pod

# Exécuter une commande dans un pod
kubectl exec -it mon-pod -- /bin/bash
kubectl exec mon-pod -- ls /app

# Copier des fichiers
kubectl cp mon-pod:/app/logs/app.log ./app.log
kubectl cp ./config.yaml mon-pod:/app/config/

# Supprimer un pod
kubectl delete pod mon-pod

# Supprimer à partir du manifeste
kubectl delete -f pod.yaml

# Forcer la suppression
kubectl delete pod mon-pod --force --grace-period=0

# Afficher les ressources consommées
kubectl top pod mon-pod

# Relancer un pod (supprime et recrée)
kubectl rollout restart deployment mon-deployment
```

---

### 6.4.3 Deployment

**Listing 6.6 – Manifeste d'un Deployment**
```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: monapp
  namespace: production
  labels:
    app: monapp
spec:
  replicas: 3
  selector:
    matchLabels:
      app: monapp
  strategy:
    type: RollingUpdate
    rollingUpdate:
      maxSurge: 1
      maxUnavailable: 0
  template:
    metadata:
      labels:
        app: monapp
        version: "2.0"
    spec:
      affinity:
        podAntiAffinity:
          preferredDuringSchedulingIgnoredDuringExecution:
          - weight: 100
            podAffinityTerm:
              labelSelector:
                matchExpressions:
                - key: app
                  operator: In
                  values:
                  - monapp
              topologyKey: kubernetes.io/hostname
      containers:
      - name: monapp
        image: monapp:2.0.0
        ports:
        - containerPort: 8080
        resources:
          requests:
            memory: "256Mi"
            cpu: "500m"
          limits:
            memory: "1Gi"
            cpu: "2000m"
        livenessProbe:
          httpGet:
            path: /actuator/health/liveness
            port: 8080
          initialDelaySeconds: 60
          periodSeconds: 15
          failureThreshold: 3
        readinessProbe:
          httpGet:
            path: /actuator/health/readiness
            port: 8080
          initialDelaySeconds: 30
          periodSeconds: 10
      terminationGracePeriodSeconds: 30
```

**Listing 6.7 – Commandes de gestion des Deployments**
```bash
# Lister les deployments
kubectl get deployments
kubectl get deploy -n production

# Créer/mettre à jour un deployment
kubectl apply -f deployment.yaml

# Décrire un deployment
kubectl describe deployment monapp

# Mettre à jour l'image d'un deployment
kubectl set image deployment/monapp monapp=monapp:3.0.0

# Mettre à l'échelle (scaling)
kubectl scale deployment monapp --replicas=5

# Autoscaling horizontal
kubectl autoscale deployment monapp \
    --min=2 --max=10 --cpu-percent=70

# Voir l'historique des rollouts
kubectl rollout history deployment monapp

# Voir les détails d'une révision spécifique
kubectl rollout history deployment monapp --revision=2

# Vérifier le statut d'un rollout
kubectl rollout status deployment monapp

# Annuler le dernier rollout
kubectl rollout undo deployment monapp

# Revenir à une révision spécifique
kubectl rollout undo deployment monapp --to-revision=3

# Mettre en pause un rollout
kubectl rollout pause deployment monapp

# Reprendre un rollout en pause
kubectl rollout resume deployment monapp

# Supprimer un deployment
kubectl delete deployment monapp
```

---

### 6.4.4 Service

**Listing 6.8 – Types de Services Kubernetes**
```yaml
# Service ClusterIP (interne au cluster)
apiVersion: v1
kind: Service
metadata:
  name: monapp-clusterip
spec:
  type: ClusterIP
  selector:
    app: monapp
  ports:
  - port: 80
    targetPort: 8080

---
# Service NodePort (accessible depuis l'extérieur via nœud)
apiVersion: v1
kind: Service
metadata:
  name: monapp-nodeport
spec:
  type: NodePort
  selector:
    app: monapp
  ports:
  - port: 80
    targetPort: 8080
    nodePort: 30080  # Port sur le nœud (30000-32767)

---
# Service LoadBalancer (cloud provider)
apiVersion: v1
kind: Service
metadata:
  name: monapp-lb
spec:
  type: LoadBalancer
  selector:
    app: monapp
  ports:
  - port: 80
    targetPort: 8080
```

**Listing 6.9 – Commandes de gestion des Services**
```bash
# Lister les services
kubectl get services
kubectl get svc

# Créer un service à partir d'un manifeste
kubectl apply -f service.yaml

# Exposer un deployment comme service
kubectl expose deployment monapp \
    --type=ClusterIP \
    --port=80 \
    --target-port=8080

# Décrire un service
kubectl describe service monapp-svc

# Accéder à un service via port-forward (développement)
kubectl port-forward service/monapp-svc 8080:80
kubectl port-forward pod/mon-pod 9090:8080

# Supprimer un service
kubectl delete service monapp-svc
```

---

### 6.4.5 ConfigMap et Secret

**Listing 6.10 – Gestion des ConfigMaps et Secrets**
```bash
# Créer un ConfigMap depuis des valeurs
kubectl create configmap app-config \
    --from-literal=APP_ENV=production \
    --from-literal=LOG_LEVEL=INFO

# Créer un ConfigMap depuis un fichier
kubectl create configmap nginx-config \
    --from-file=nginx.conf

# Créer un ConfigMap depuis un répertoire
kubectl create configmap app-configs \
    --from-file=./configs/

# Lister les ConfigMaps
kubectl get configmaps
kubectl get cm

# Afficher le contenu d'un ConfigMap
kubectl describe configmap app-config
kubectl get configmap app-config -o yaml

# Créer un Secret opaque
kubectl create secret generic db-secret \
    --from-literal=username=admin \
    --from-literal=password=MonMotDePasse123!

# Créer un Secret depuis un fichier
kubectl create secret generic tls-secret \
    --from-file=tls.crt=./certs/server.crt \
    --from-file=tls.key=./certs/server.key

# Secret de type TLS
kubectl create secret tls mon-tls \
    --cert=./certs/server.crt \
    --key=./certs/server.key

# Secret de type Docker Registry
kubectl create secret docker-registry regcred \
    --docker-server=registry.exemple.com \
    --docker-username=mon-user \
    --docker-password=mon-mdp \
    --docker-email=contact@exemple.com

# Lister les secrets
kubectl get secrets

# Décoder un secret (base64)
kubectl get secret db-secret -o jsonpath='{.data.password}' | base64 -d

# Supprimer un ConfigMap / Secret
kubectl delete configmap app-config
kubectl delete secret db-secret
```

---

### 6.4.6 PersistentVolume et PersistentVolumeClaim

**Listing 6.11 – PersistentVolume et PersistentVolumeClaim**
```yaml
# PersistentVolume (PV)
apiVersion: v1
kind: PersistentVolume
metadata:
  name: mon-pv
spec:
  capacity:
    storage: 10Gi
  volumeMode: Filesystem
  accessModes:
  - ReadWriteOnce
  persistentVolumeReclaimPolicy: Retain
  storageClassName: standard
  hostPath:
    path: /mnt/data

---
# PersistentVolumeClaim (PVC)
apiVersion: v1
kind: PersistentVolumeClaim
metadata:
  name: mon-pvc
spec:
  accessModes:
  - ReadWriteOnce
  resources:
    requests:
      storage: 5Gi
  storageClassName: standard
```

**Listing 6.12 – Commandes PV et PVC**
```bash
# Lister les PersistentVolumes
kubectl get pv

# Lister les PersistentVolumeClaims
kubectl get pvc

# Décrire un PVC
kubectl describe pvc mon-pvc

# Supprimer un PVC
kubectl delete pvc mon-pvc
```

---

### 6.4.7 Ingress

**Listing 6.13 – Manifeste Ingress**
```yaml
apiVersion: networking.k8s.io/v1
kind: Ingress
metadata:
  name: mon-ingress
  annotations:
    nginx.ingress.kubernetes.io/rewrite-target: /
    nginx.ingress.kubernetes.io/ssl-redirect: "true"
spec:
  ingressClassName: nginx
  tls:
  - hosts:
    - app.exemple.com
    secretName: mon-tls
  rules:
  - host: app.exemple.com
    http:
      paths:
      - path: /api
        pathType: Prefix
        backend:
          service:
            name: api-service
            port:
              number: 80
      - path: /
        pathType: Prefix
        backend:
          service:
            name: frontend-service
            port:
              number: 80
```

---

## 6.5 Commandes Générales kubectl

**Listing 6.14 – Commandes générales kubectl**
```bash
# Obtenir toutes les ressources d'un namespace
kubectl get all -n mon-namespace

# Appliquer des modifications (create ou update)
kubectl apply -f manifeste.yaml

# Appliquer tous les manifestes d'un répertoire
kubectl apply -f ./k8s/

# Voir les différences avant application
kubectl diff -f manifeste.yaml

# Supprimer des ressources
kubectl delete -f manifeste.yaml

# Obtenir des ressources au format JSON/YAML
kubectl get deployment monapp -o yaml
kubectl get pods -o json

# Filtrer avec jsonpath
kubectl get pods -o jsonpath='{.items[*].metadata.name}'

# Filtrer avec custom-columns
kubectl get pods \
    -o custom-columns=NOM:.metadata.name,STATUT:.status.phase

# Filtrer par label
kubectl get pods -l app=monapp
kubectl get pods -l 'env in (prod,staging)'

# Étiqueter une ressource
kubectl label pod mon-pod environment=production

# Annoter une ressource
kubectl annotate pod mon-pod \
    description="Pod de production critique"

# Voir les événements du cluster
kubectl get events --sort-by='.lastTimestamp'
kubectl get events -n mon-namespace

# Afficher les ressources consommées par les nœuds
kubectl top nodes

# Afficher les ressources consommées par les pods
kubectl top pods

# Appliquer un correctif (patch)
kubectl patch deployment monapp \
    -p '{"spec":{"replicas":5}}'

# Éditer une ressource directement
kubectl edit deployment monapp
```

---

## 6.6 Helm – Gestionnaire de Paquets Kubernetes

**Listing 6.15 – Commandes Helm essentielles**
```bash
# Installer Helm
curl https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3 | bash

# Vérifier la version
helm version

# Ajouter un dépôt de charts
helm repo add stable https://charts.helm.sh/stable
helm repo add bitnami https://charts.bitnami.com/bitnami

# Mettre à jour les dépôts
helm repo update

# Lister les dépôts
helm repo list

# Rechercher un chart
helm search repo nginx

# Afficher les valeurs par défaut d'un chart
helm show values bitnami/nginx

# Installer un chart
helm install mon-nginx bitnami/nginx

# Installer avec des valeurs personnalisées
helm install mon-nginx bitnami/nginx \
    --set service.type=NodePort \
    --set replicaCount=2 \
    -n production --create-namespace

# Installer avec un fichier de valeurs
helm install mon-nginx bitnami/nginx \
    -f mes-valeurs.yaml

# Mettre à jour un déploiement Helm
helm upgrade mon-nginx bitnami/nginx --set replicaCount=3

# Installer ou mettre à jour (upsert)
helm upgrade --install mon-nginx bitnami/nginx \
    -f mes-valeurs.yaml

# Lister les releases
helm list
helm ls -n production

# Voir l'historique d'une release
helm history mon-nginx

# Revenir à une version précédente
helm rollback mon-nginx 1

# Désinstaller une release
helm uninstall mon-nginx

# Créer un nouveau chart
helm create mon-chart

# Valider un chart
helm lint mon-chart/

# Générer le YAML sans déployer (debug)
helm template mon-nginx bitnami/nginx -f mes-valeurs.yaml
```

---

# Chapitre 7 — Infrastructure as Code

---

## 7.1 Introduction

> **Infrastructure as Code (IaC) :** pratique consistant à décrire et à gérer l'infrastructure informatique (serveurs, réseaux, bases de données, etc.) sous forme de **fichiers de configuration versionnables et automatisables**, plutôt que par des interventions manuelles.

**Avantages de l'IaC :**

- Reproductibilité et cohérence entre les environnements.
- Versionnage et traçabilité des modifications.
- Automatisation et rapidité de provisionnement.
- Réduction des erreurs humaines.
- Documentation vivante de l'infrastructure.

---

## 7.2 Terraform

### 7.2.1 Présentation

**Terraform**, développé par HashiCorp, est l'outil IaC le plus populaire. Il supporte des dizaines de fournisseurs cloud (AWS, Azure, GCP, etc.) et utilise le langage **HCL** (*HashiCorp Configuration Language*).

### 7.2.2 Installation

**Listing 7.1 – Installation de Terraform**
```bash
# Méthode 1 : via le gestionnaire de paquets HashiCorp
wget -O- https://apt.releases.hashicorp.com/gpg | \
    sudo gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-keyring.gpg

echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] \
    https://apt.releases.hashicorp.com $(lsb_release -cs) main" | \
    sudo tee /etc/apt/sources.list.d/hashicorp.list

sudo apt-get update && sudo apt-get install -y terraform

# Vérifier l'installation
terraform version

# Complétion bash
terraform -install-autocomplete
```

### 7.2.3 Commandes Terraform

**Listing 7.2 – Cycle de vie Terraform**
```bash
# Initialiser le répertoire de travail
terraform init

# Initialiser avec mise à jour des providers
terraform init -upgrade

# Formater le code HCL
terraform fmt

# Formater récursivement
terraform fmt -recursive

# Valider la syntaxe
terraform validate

# Planifier les modifications (dry-run)
terraform plan

# Sauvegarder le plan dans un fichier
terraform plan -out=monplan.tfplan

# Appliquer les modifications
terraform apply

# Appliquer un plan sauvegardé
terraform apply monplan.tfplan

# Appliquer sans confirmation
terraform apply -auto-approve

# Passer des variables
terraform apply -var="region=eu-west-1" -var="instance_count=3"

# Appliquer avec fichier de variables
terraform apply -var-file="prod.tfvars"

# Détruire l'infrastructure
terraform destroy

# Détruire sans confirmation
terraform destroy -auto-approve

# Détruire une ressource spécifique
terraform destroy -target=aws_instance.mon_serveur

# Afficher l'état actuel
terraform show

# Lister les ressources dans l'état
terraform state list

# Afficher une ressource spécifique dans l'état
terraform state show aws_instance.mon_serveur

# Déplacer une ressource dans l'état
terraform state mv aws_instance.ancien aws_instance.nouveau

# Retirer une ressource de l'état (sans la supprimer)
terraform state rm aws_instance.mon_serveur

# Importer une ressource existante
terraform import aws_instance.mon_serveur i-0123456789abcdef0

# Afficher les outputs
terraform output
terraform output nom_du_output

# Graphe de dépendances
terraform graph | dot -Tsvg > graph.svg

# Verrouiller/déverrouiller l'état
terraform force-unlock LOCK_ID

# Mettre à jour les modules
terraform get -update

# Tester les expressions
terraform console
```

### 7.2.4 Exemple de Configuration Terraform

**Listing 7.3 – Exemple infrastructure AWS avec Terraform (main.tf)**
```hcl
# Configuration du provider
terraform {
  required_version = ">= 1.0"
  required_providers {
    aws = {
      source  = "hashicorp/aws"
      version = "~> 5.0"
    }
  }
  backend "s3" {
    bucket = "mon-tfstate"
    key    = "production/terraform.tfstate"
    region = "eu-west-1"
  }
}

provider "aws" {
  region = var.region
  default_tags {
    tags = {
      Environment = var.environment
      ManagedBy   = "Terraform"
    }
  }
}

# Variables
variable "region" {
  type    = string
  default = "eu-west-1"
}

variable "environment" {
  type = string
}

variable "instance_count" {
  type    = number
  default = 2
}

# Ressources
resource "aws_vpc" "principal" {
  cidr_block           = "10.0.0.0/16"
  enable_dns_hostnames = true
  tags = { Name = "vpc-${var.environment}" }
}

resource "aws_instance" "serveur" {
  count         = var.instance_count
  ami           = data.aws_ami.ubuntu.id
  instance_type = "t3.micro"
  subnet_id     = aws_subnet.public.id
  tags = { Name = "serveur-${var.environment}-${count.index}" }
}

# Outputs
output "instance_ips" {
  value = aws_instance.serveur[*].public_ip
}
```

---

## 7.3 Ansible

### 7.3.1 Présentation

**Ansible** est un outil d'automatisation *agentless* (sans agent) qui permet de configurer des systèmes, de déployer des applications et d'orchestrer des tâches complexes. Il utilise **SSH** pour communiquer avec les machines cibles.

### 7.3.2 Installation

**Listing 7.4 – Installation d'Ansible**
```bash
# Ubuntu / Debian
sudo apt-get update
sudo apt-get install -y software-properties-common
sudo add-apt-repository --yes --update ppa:ansible/ansible
sudo apt-get install -y ansible

# Via pip
pip install ansible --break-system-packages

# Vérifier l'installation
ansible --version
```

### 7.3.3 Commandes Ansible

**Listing 7.5 – Commandes Ansible**
```bash
# Tester la connectivité (ping)
ansible all -i inventaire.ini -m ping
ansible webservers -i inventaire.ini -m ping

# Exécuter une commande ad-hoc
ansible all -i inventaire.ini -m command -a "uptime"
ansible all -i inventaire.ini -m shell -a "df -h"
ansible webservers -i inventaire.ini -m service \
    -a "name=nginx state=restarted" --become

# Copier un fichier
ansible all -i inventaire.ini -m copy \
    -a "src=fichier.conf dest=/etc/app/fichier.conf"

# Installer un paquet
ansible all -i inventaire.ini -m apt \
    -a "name=nginx state=present" --become

# Exécuter un playbook
ansible-playbook -i inventaire.ini playbook.yml

# Exécuter en mode dry-run (check)
ansible-playbook -i inventaire.ini playbook.yml --check

# Afficher les différences
ansible-playbook -i inventaire.ini playbook.yml --diff

# Limiter l'exécution à un groupe
ansible-playbook -i inventaire.ini playbook.yml \
    --limit webservers

# Passer des variables extra
ansible-playbook -i inventaire.ini playbook.yml \
    -e "env=production version=2.0.0"

# Afficher les tâches disponibles
ansible-playbook playbook.yml --list-tasks

# Afficher les hôtes cibles
ansible-playbook playbook.yml --list-hosts

# Exécuter avec plus de verbosité
ansible-playbook -i inventaire.ini playbook.yml -v
ansible-playbook -i inventaire.ini playbook.yml -vvv

# Vérifier la syntaxe d'un playbook
ansible-playbook playbook.yml --syntax-check

# Gestion des rôles (Galaxy)
ansible-galaxy role install geerlingguy.nginx
ansible-galaxy collection install community.docker
ansible-galaxy list

# Initialiser un nouveau rôle
ansible-galaxy role init mon-role

# Chiffrer un fichier avec Vault
ansible-vault encrypt secrets.yml
ansible-vault decrypt secrets.yml
ansible-vault view secrets.yml
ansible-vault edit secrets.yml

# Exécuter avec Vault
ansible-playbook playbook.yml --ask-vault-pass
ansible-playbook playbook.yml \
    --vault-password-file ~/.vault_pass
```

---



