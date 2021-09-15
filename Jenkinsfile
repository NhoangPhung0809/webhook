pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('Test Python') {
            steps{
                echo 'Python test.!.!.!.!.!.'
                sh 'python --version'
                sh 'install python3-pip'
                }
            }
        stage('install django') {
            steps {
                echo 'Install....'
                sh 'pip3 install Django' 
        stage('build') {
            steps {
                echo 'Build.......'
                sh 'python manage.py'
            }
        }
    }
}
