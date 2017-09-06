pipeline {
    agent none
    stages {
        stage('Back-end') {
            agent {
                docker { image 'java:openjdk-7-jdk-alpine' } 
            }
            steps {
                sh 'java -version'
            }
        }
        stage('Front-end') {
            agent {
                docker { image 'node:7-alpine' }
            }
            steps {
                sh 'node --version'
            }
        }
    }
}