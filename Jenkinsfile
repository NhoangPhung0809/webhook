pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('Test...Python') {
            steps{
                env.WORKSPACE = pwd()
                echo 'Python test.!.!.!.!.!.'
                sh 'python --version'
                sh 'virtualenv --python=python34 venv'
                sh 'pip install -r requirements.txt'
                }
            }
        stage('install...django...') {
            steps {
                echo 'Install....'
                sh 'pip install Django' 
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
