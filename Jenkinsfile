pipeline {
    agent any
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
        success {
            echo "This is success status"
        }
        failure {
            echo "This is failure status"
        }
    }
}