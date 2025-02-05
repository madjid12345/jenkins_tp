pipeline {
    agent any
    stages {
        stage('Cloner le dépôt') {
            steps {
                git 'https://github.com/nom-utilisateur/nom-repo.git'
            }
        }
        stage('Installer les dépendances') {
            steps {
                sh 'npm install'
            }
        }
        stage('Tests') {
            steps {
                sh 'npm test'
            }
        }
        stage('Déploiement') {
            steps {
                sh 'npm run deploy'
            }
        }
    }
}
