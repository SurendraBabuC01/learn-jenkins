pipeline {

  agent {
    node {
      label 'workstation'
    }
  }

  environment {
    env_variable = 'env_variable'
  }

  stages {

    stage('One') {

      steps {
        sh 'echo surendra'
      }
    }

    stage('Two') {

          steps {
            sh 'echo env_variable - "${env_variable}"'
          }
        }
  }

  post {
    always {
      echo 'Clean SetUP Pipeline'
    }
  }
}