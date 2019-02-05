pipeline {
    agent any
    environment { 
        Integration = 'true'
        env.NODEPATH = '/Users/a206105996/.jenkins/tools/jenkins.plugins.nodejs.tools.NodeJSInstallation/NodejS_10.4.1'
    }
    stages {
        stage('Build') {
            steps {
                sh '''
                PATH="$PATH:$NODEPATH"
                echo "Path is set to " $PATH
                npm install --no-optional 
                   npm install
                   '''
            }
        }
        stage('Unit Test') {
            steps {
                sh '''
                PATH="$PATH:$NODEPATH"
                echo "Path is set to " $PATH
                npm install --no-optional 
                   npm test
                   '''
            }
        }
    }
}
