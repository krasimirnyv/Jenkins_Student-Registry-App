pipeline {
    agent any

    environment {
        PATH = "/usr/local/opt/node/bin:${env.PATH}"
    }

    stages {
        stage("Install Dependencies") {
            steps {
                sh  'npm install'
            }
        }
        stage("Run Tests") {
            steps {
                sh  'npm run test'
            }
        }
    }
}