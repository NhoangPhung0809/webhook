pipeline {
    agent { docker { image 'python:3.9.7' } }
    stages {
        stage {
            sh 'chmod -R 777 /.local'
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
                sh 'python -m pip install Django' 
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
