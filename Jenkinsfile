pipeline {
    agent any

    stages {
        stage('Check Yarn Version') {
            steps {
                sh 'yarn --version'
            }
        }

        stage('Install Dependencies') {
            steps {
                // Checkout your source code from a Git repository if needed
                // git branch: 'your-branch', url: 'your-git-repo-url'

                // Run 'yarn install'
                sh 'yarn install'
            }
        }
    }
}