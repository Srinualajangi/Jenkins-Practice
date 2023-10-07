// pipeline {
//     agent { node { label 'AGENT-1' } }
//     stages {
//         stage ('Build') {
//             steps {
//                  echo 'Building..'
//               sh '''
//                 ls -ltr
//                 pwd
//                 echo "Hello from Sample Pipeline"
//                 printenv
//               '''
//             }
//         }
//     }
//         stage ('Test') {
//         steps {
//             echo 'Testing'
//         }
//     }
    
//         stage ('Deploy') {
//         steps {
//             echo 'Deploying...'
//         }
//     }
// }

pipeline {
    agent { node { label 'AGENT-1' } }
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
              sh '''
                ls -ltr
                pwd
                echo "Hello from Sample Pipeline"
                printenv
              '''
            }
        }
        stage('Test') {
            steps {
                echo 'Testing'
            }
        }
        stahjge('Deploy') {
            steps {
                echo 'Deploying..'
            }
        }
    }
    post { 
        always { 
            echo 'I will always say Hello again!'
        }
        success {
            echo 'I will run at successs'
        }
        failure {
            echo 'I will run at failures'
        }
    }
}