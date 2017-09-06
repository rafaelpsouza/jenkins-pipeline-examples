pipeline {
    agent any 

    environment { 
        GLOBAL_VAR = 'My Global Var'
    }

    stages {
        stage('Build') { 
            environment { 
                MY_STAGE_VAR = credentials('0de54e42-04c8-4590-86af-b2b96ad3f56f')
            }
            steps {
                 sh 'printenv'
            }
        }
    }
}