pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
         stage('update') {
            steps {
                sh 'chmod -R 777 ./cache/pip/'
                echo 'update.......'
                sh 'pip install --upgrade pip'
            }
        }
        stage('Test...Python') {
            steps{
                echo 'Python test.!.!.!.!.!.'
                sh 'python --version'
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
