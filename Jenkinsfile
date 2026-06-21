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
                sh 'hello'
            }
        }
        stage (Deploy) {
            steps {
                echo "Deploying..."
            }
        }
    }
    post {
        always {
            echo "this is always"
        }
        success {
            echo "This is success status"
        }
        failure {
            echo "This is failure status"
        }
    }
}