pipeline {
    agent any
    stages {
        stage('install...django...') {
            steps {
                dir('./var/lib/jenkins/workspace/project-website/env/bin/'){
                    echo 'Python test.!.!.!.!.!.'
                    sh 'python --version'
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
