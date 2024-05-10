pipeline {
    agent any

    stages {
        stage('Remove Existing Clone') {
            steps {
                // Remove existing clone, if any
                deleteDir()
            }
        }

        stage('Clone Repository') {
            steps {
                // Clone GitHub repository
                git ''
            }
        }

        stage('Build') {
            steps {
                // Run your build steps
                bat 'MyWorld.py'
            }
        }
    }
}
