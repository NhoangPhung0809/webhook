pipeline {
    agent { docker { image 'python:3.9.7' } }
    stages {
        stage('Test...Python') {
            steps{
                sh 'python3 -m venv env'
                echo 'Python test.!.!.!.!.!.'
                sh 'python --version'
 
                }
            }
        stage('install...django...') {
            steps {
                echo 'Install....'
                sh 'pip3 install Django' 
                }
            }
        stage('build') {
            steps {
                echo 'Build.......'
                sh 'python manage.py'
            }
        }
    }
}
