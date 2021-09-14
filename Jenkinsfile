pipeline {
    agent any
    tools {
        python 'python'
    }
    stages {
        stage('Test...') {
            steps {
                sh 'python --version'
            }
        }
        stage('build...') {
            steps {
                sh 'python manage.py'
            }
        }
    }
}
