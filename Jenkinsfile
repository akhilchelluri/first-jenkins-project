pipeline {
    agent {
        docker {
            image 'node:15'
        }
    }

    stages {
        stage('Check Version') {
            steps {
                sh 'node -v'
            }
        }

        stage('Run App') {
            steps {
                sh 'node app.js'
            }
        }
    }
}
