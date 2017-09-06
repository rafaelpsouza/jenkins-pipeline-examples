pipeline {
    agent { 
    	docker { image 'java:openjdk-7-jdk-alpine' } 
    }
    stages {
        stage('Test') {
            steps {
                sh 'java -version'
            }
        }
    }
}