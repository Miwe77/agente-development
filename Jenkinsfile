pipeline {
   
    agent{
        node {
            label 'Development'
        }
    }
    stages {
        stage('Build') {
            steps {
                echo "Building ... in the node ${NODE_NAME}  and in the executor ${EXECUTOR_NUMBER}"
                sh 'uname -n'
            }
        }
        stage('Test') {
            steps {
                echo "Testing ... in the node ${NODE_NAME}  and in the executor ${EXECUTOR_NUMBER}"
                sh 'uname -n'
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying ... in the node ${NODE_NAME}  and in the executor ${EXECUTOR_NUMBER}"  
                sh 'uname -n'
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
