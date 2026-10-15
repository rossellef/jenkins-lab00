pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                dir('demo-app') {
                    echo '🛠️ Build en cours...'
                    sh 'mvn clean compile'
                }
            }
        }
        stage('Test') {
            steps {
                dir ('demo-app') {
                    echo '✅ Tests unitaires...'
                    sh 'mvn test'
                }
            }
        }
    }
}