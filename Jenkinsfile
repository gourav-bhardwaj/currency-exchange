pipeline {
    agent any
    tools {
        maven "Maven"
    }
    stages {
        stage('Checkout') {
            steps {
                echo "Checkout work is in progress..."
                checkout([$class: 'GitSCM', branches: [[name: "${BRANCH_NAME}"]], extensions: [], userRemoteConfigs: [[credentialsId: 'GIT_CREDS', url: 'https://github.com/gourav-bhardwaj/currency-exchange.git']]])
            }
        }
    }
}
