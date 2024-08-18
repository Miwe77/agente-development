pipeline {
    agent {
        node {
            label 'Development'
        }
    }
    stages {
        stage('Build') {
            steps {
                echo "Building... in ${NODE_NAME}"
                
            }
        }
        stage('Test') {
            steps {
                echo "Testing... in ${NODE_NAME}"
                
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying... in ${NODE_NAME}"                
            }
        }
    }
    post {
        always {
            echo 'This will always run'
        }
        success {
            echo 'This will run only if the pipeline succeeds'
        }
        failure {
            echo 'This will run only if the pipeline fails'
        }
    }
}
