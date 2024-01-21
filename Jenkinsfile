pipeline {
    agent any

    tools {
        maven 'Maven3' // Replace with your Maven version
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package' // Adjust the Maven command as needed
            }
        }

        // You can add more stages for testing, deployment, etc.
    }

    post {
        always {
            echo 'Build completed'
        }
    }
}
