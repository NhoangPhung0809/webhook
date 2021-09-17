pipeline {
    agent any
    stages {
        stage('Test...Python') {
            steps {
                echo 'Python test.!.!.!.!.!.'
                sh 'install python3.7'
                sh 'python --version'
                }
            }
        stage('install...django...') {
            steps {
                dir('./var/lib/jenkins/workspace/project-website/env/bin/'){
                    echo 'qua'
                }
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
