pipeline {
    agent any  // Run on any available Jenkins agent

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/Saloni899/user-management.git'
            }
        }

        stage('Build') {
            steps {
                sh './mvnw clean package'  // Adjust based on your project (Maven, Gradle, etc.)
            }
        }

        stage('Test') {
            steps {
                sh './mvnw test'  // Run unit tests (if applicable)
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                // Add deployment steps here (Docker, Kubernetes, etc.)
            }
        }
    }
}
