pipeline {
    agent { node { label 'AGENT-1' } }
    stages {
        stage ('Build') {
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
    }
        stage ('Test') {
        steps {
            echo 'Testing'
        }
    }
    
       stage ('Deploy') {
        steps {
            echo 'Deploying...'
        }
    }
}