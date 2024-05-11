pipeline {
    agent any
    
    stages {
        stage('Remove Old Clone') {
            steps {
                // Delete the old cloned repository
                script {
                    sh 'rm -rf C:/Windows/System32/ToCS'
                }
            }
        }
        
        stage('Clone Repository') {
            steps {
                
                git 'https://github.com/YusraNawaz054/ToCS.git'
            }
        }
        
        stage('Build Python File') {
            steps {
                
                bat 'MyWorld.py'
            }
        }
    }
}
