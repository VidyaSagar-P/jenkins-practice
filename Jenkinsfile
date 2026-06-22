pipeline {
    // agent any
    agent {
        label 'AGENT-1'
    }
    stages {
        stage ('Build') {
            steps {
                echo "Building..."
            }
        }
        stage ('Test') {
            steps {
                echo "Testing..."
                // sh 'hello'
            }
        }
        stage (Deploy) //this will work without single quotes also
         {
            steps {
                echo "Deploying..."
            }
        }
    }



    // Post build actions
    post {
        always {
            echo "always"
        }
        success {
            echo "This is success status"
        }
        failure {
            echo "This is failure status"
        }
    }
}