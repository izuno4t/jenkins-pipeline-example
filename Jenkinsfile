pipeline {
    agent { 
        docker { 
            image 'maven:3.6.1-jdk-8-slim'
            args '-v $HOME/.m2:/root/.m2'
        } 
    }
    stages {
        stage('build') {
            steps {
                sh 'mvn clean site'
            }
        }
    }
}