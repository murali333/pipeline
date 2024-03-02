pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        script {
                  checkout scm
                }
      }
    }
     stage('build') {
          steps {
            script {
                       sh 'mvn clean package'
                    }
          }
        }

  }
  environment {
    env = 'dev'
  }
}