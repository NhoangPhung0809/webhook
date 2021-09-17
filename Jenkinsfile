pipeline {
    agent any
    stages {
        stage('check Vesion') {
            steps {
                dir('./var/lib/jenkins/workspace/project-website/env/bin/'){
                    echo 'Python test.!.!.!.!.!.'
                    sh 'python3 --version'
                }
            }
        }
        stage('build') {
            steps {
                echo 'Build.......'
                sh 'python3 manage.py'
            }
        }
    }
}
