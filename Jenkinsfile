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
        stage('Deploy DEV') {
            steps {
                // sh 'make publish'
                echo 'Deploying ...'
            }
        }

        stage('Deploy PROD') {
            steps {
                timeout(time:1, unit:'DAYS') {
                    input message: 'Are you sure?'
                } 
                echo 'Deploying ...'
            }
        }
    }
}