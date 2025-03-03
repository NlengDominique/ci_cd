pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/NlengDominique/ci_cd.git'
            }
        }

        stage('Build') {
            steps {
                sh 'npm install'
                sh 'npm run build'
            }
        }

        stage('Test') {
            steps {
                sh 'npm run test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Déploiement sur Vercel à venir...'
            }
        }
    }
}
