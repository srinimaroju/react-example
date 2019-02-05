pipeline {
    agent
    environment { 
        Integration = 'true'
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Unit Test') {
            steps {
                sh 'npm test'
            }
        }
    }
}
