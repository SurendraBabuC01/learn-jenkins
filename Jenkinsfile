pipeline {

  agent {
    node {
      label 'workstation'
    }
  }

  environment {
    env_variable = 'env_variable'
  }

  input {
    message "Should we continue?"
    ok "Yes"
    parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Please provide the input?')
      }
  }

  options {
     ansiColor('xterm')
  }

  triggers { pollSCM('H/2 * * * *') }

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

    stage('Three') {

              steps {
                echo "Hello ${params.PERSON}"
              }
            }
  }

  post {
    always {
      echo 'Clean SetUP Pipeline'
    }
  }
}

