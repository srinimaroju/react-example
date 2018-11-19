pipeline {
  agent {
    node {
      label 'Integration'
    }

  }
  stages {
    stage('SCM') {
      steps {
        sh 'npm install'
      }
    }
  }
}