pipeline {
    agent any 

    stages {
        stage('Build') { 
            steps { 
                // sh 'make'
                echo 'Building ...'
            }
        }
        stage('Test'){
            steps {
                // sh 'make check'
                // junit 'reports/**/*.xml'
                echo 'Testing ...'
            }
        }
        stage('Deploy') {
            steps {
                // sh 'make publish'
                echo 'Deploying ...'
            }
        }
    }
}