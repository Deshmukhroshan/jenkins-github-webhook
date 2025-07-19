pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning repo...'
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'chmod +x hello.sh && ./hello.sh'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests... (mock)'
            }
        }
    }

    post {
        success {
            echo '✅ Pipeline completed successfully!'
        }
        failure {
            echo '❌ Pipeline failed.'
        }
    }
}
