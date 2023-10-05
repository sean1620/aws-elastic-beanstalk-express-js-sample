pipeline {
    agent {
        docker {
            image 'node:16'
        }
    }

    stages {
        stage('Build') {
            steps {
                sh 'npm install --save'
            }
        }
    }

    post {
        always {
            // This step will always be executed, even if the build fails.
            echo 'Build finished.'
        }
    }
}
