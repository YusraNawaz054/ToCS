pipeline {
    agent any
    
    stages {
        stage('Delete Old Cloned Repository') {
            steps {
                deleteDir()
            }
        }
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/YusraNawaz054/ToCS.git'
            }
        }
        stage('Build') {
            steps { 
                bat 'MyWorld.py'
            }
        }
    }
}
