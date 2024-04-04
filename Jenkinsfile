pipeline { 
    agent {
        label 'ws'
    }
    stages {
        stage('Lint Checks') {
            steps {
                sh "echo Installing Lint Checker"
                sh "npm i jslint"
                sh "node_modules/jslint/bin/jslint.js server.js || true" 
            }
        }

        stage('Static Code Analysis') {
            steps {
                sh "echo Static Checks ...."
            }
        }

    }
}