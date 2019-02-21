pipeline {
    agent any
    triggers{ cron('* * * * *') }
    triggers{ pollSCM('H */4 * * 1-5') }
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
