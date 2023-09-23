pipeline {
    agent any // You can specify a specific agent label here if needed

    stages {
        stage('Checkout') {
            steps {
                // This step checks out your source code repository
                checkout scm
            }
        }

        stage('Yarn Install') {
            steps {
                // This step runs a Windows batch command to execute 'yarn install'
                bat 'npm install'
            }
        }
    }

    post {
        success {
            // This block will be executed if the pipeline succeeds
            echo 'Yarn install succeeded'
        }

        failure {
            // This block will be executed if the pipeline fails
            echo 'Yarn install failed'
        }
    }
}
