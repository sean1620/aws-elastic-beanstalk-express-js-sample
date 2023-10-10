pipeline {
    agent {
        docker {
            image 'node:16'
            args '-u root:root' // to override user to root if needed
        }
    }
    stages {
        stage('Build') {
            steps {
                script {
                    sh 'npm install --save'
                }
            }
        }
    }
    post {
        always {
            echo 'Build complete!'
        }
    }
}
