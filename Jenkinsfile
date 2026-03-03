pipeline {
    agent {
        docker {
            image 'node:14'
        }
    }

    stages {
        stage('Check Version') {
            steps {
                sh 'node -v'
            }
        }

     stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Run App') {
            steps {
                sh 'npm start'
            }
        }
    }
}
