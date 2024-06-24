pipeline {
    agent any

    stages {
        stage('Identify Branch') {
            steps {
                script {
                    def branchName = env.BRANCH_NAME
                    echo "Current branch is: ${branchName}"
                }
            }
        }
        stage('Build') {
            steps {
                echo "Building the project on branch: ${env.BRANCH_NAME}"
            }
        }
        stage('Test') {
            steps {
                echo "Running tests on branch: ${env.BRANCH_NAME}"
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying the project from branch: ${env.BRANCH_NAME}"
            }
        }
    }
}

