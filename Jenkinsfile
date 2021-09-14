pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('Test Python') {
            steps{
                echo 'Python test......'
                sh 'pythn --version'
        stage('build.!.!.!.') {
            steps {
                echo 'Build.......'
                sh 'python manage.py'
            }
        }
    }
}
