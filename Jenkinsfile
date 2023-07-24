pipeline {
    agent any

    sh 'printenv'
    environment {
        IRONIC_NUM = 0.0
    }
    stages {
        stage('Build') {
            when {
                expression {
                    BRANCH_NAME == 'hotfix_*' && 
                }
            }   
            steps {
                echo 'Building...'
                // Add your build steps here
            }
        }
        
        stage('Test') {
            steps {
                echo 'Testing...'
                // Add your test steps here
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Add your deployment steps here
            }
        }
    }

    post {
        always {

        }
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
