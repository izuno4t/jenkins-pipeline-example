pipeline {
    agent { docker { image 'maven:3.6.1' } }
    stages {
        stage('clean') {
            steps {
                sh './mvnw clean'
            }
        }
        stage('site') {
            steps {
                sh './mvnw site'
            }
        }
    }
}