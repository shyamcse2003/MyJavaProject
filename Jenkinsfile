pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello, World!'
            }
        }

        stage('cat README') {
            when {
                expression { env.BRANCH_NAME.startsWith('s') }
            }
            steps {
                script {
                    sh 'cat README.md'
                }
            }
        }
    }
}

