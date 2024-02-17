// pipeline {
//
//   agent {
//     node {
//       label 'workstation'
//     }
//   }

//   environment {
//     env_variable = 'env_variable'
//   }
//
//    parameters {
//      string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Please provide the input?')
//    }

  options {
     ansiColor('xterm')
  }

//   triggers { pollSCM('H/2 * * * *') }

//   stages {
//
//     stage('parallel stage') {
//       parallel {
//         stage('One') {
//               input {
//                 message "Should we continue?"
//                 ok "Yes"
//               }
//               steps {
//                 sh 'echo surendra'
//               }
//             }
//
//             stage('Two') {
//                    when {
//                      expression {
//                        GIT_BRANCH == "origin/test"
//                      }
//                    }
//                   steps {
//                     sh 'echo env_variable - "${env_variable}"'
//                   }
//                 }
//
//             stage('Three') {
//
//                       steps {
//                         echo "Hello ${params.PERSON}"
//                       }
//                     }
//
//       }
//     }
//   }
//
//   post {
//     always {
//       echo 'Clean SetUP Pipeline'
//     }
//   }
// }


pipeline {

  agent {
    node {
      label 'workstation'
    }
  }

  stages {
    stage('One') {
      echo 'Hello World'
    }
  }

  }

