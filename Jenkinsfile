pipeline {
    agent any
    stages {
        stage('Test...Python') {
            agent { docker { image 'python:3.9.7' } }
            steps {
                echo 'Python test.!.!.!.!.!.'
                sh 'python --version'
                }
            }
        stage('install...django...') {
            steps {
                dir('./var/lib/jenkins/workspace/project-website/env/bin/'){
                    sh 'apt install python3.9-venv'
                    sh 'python3 -m venv env'
                    echo 'Install....'
                    sh 'pip3 install Django' 
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
