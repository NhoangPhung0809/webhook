pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
         stage('update') {
            steps {
                echo 'Update.......'
                sh 'mkdir /.cache/pip'
                sh 'touch http '
                
            }
         }
        stage('Test...Python') {
            steps{
                echo 'Python test.!.!.!.!.!.'
                sh 'python --version'
                sh 'pip install -r requirements.txt'
                }
            }
        stage('install...django...') {
            steps {
                echo 'Install....'
                sh 'pip install -r Django' 
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
