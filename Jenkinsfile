pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('Test....') {
            sh 'python --version'
        }
        stage('build') {
            steps {
                sh 'python manage.py'
            }
        }
    }
}
