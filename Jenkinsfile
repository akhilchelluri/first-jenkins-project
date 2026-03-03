pipeline {
    agent {
        docker {
            image 'node:14'
        }
    }
     environment {
    HOME = "${WORKSPACE}"
    NPM_CONFIG_CACHE = "${WORKSPACE}/.npm"
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
