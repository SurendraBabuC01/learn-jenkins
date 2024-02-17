pipeline {

  agent {
    node {
      label 'workstation'
    }
  }

  environment {
    env_variable = 'env_variable'
  }

  parameters {
    string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Please provide the input?')
  }

  options {
     ansiColor('xterm')
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