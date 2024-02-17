pipeline {

  agent {
    node {
      label 'workstation'
    }
  }

  stages {

    stage('one') {

      steps {
        sh 'echo surendra'
      }
    }
  }

  post {
    always {
      echo 'Clean SetUP Pipeline'
    }
  }
}