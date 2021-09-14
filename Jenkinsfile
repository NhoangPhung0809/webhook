pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('Test...') {
            steps {
                sh 'python --version'
                echo 'toi day chua'
            }
        }
        stage('build...') {
            steps {
                sh 'python manage.py'
            }
        }
    }
}
