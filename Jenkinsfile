pipeline {
    agent {
        docker { image 'node:12-alpine' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'npm install'
                sh 'npm test'
            }
        }
    }
}
