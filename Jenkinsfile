pipeline {
    agent any 
    stages {
        stage('List Files in Repo') {
            steps {
                echo "Cloning branch: ${ env.BRANCH_NAME }" 
                sh 'ls -lart' 
            }
        }
    }
    post {
        always {
            echo 'Pipeline finished for branch ' + env.BRANCH_NAME
        }
    }
}