pipeline {
    agent {docker image{'python:3.5.1'}}
    stages {
        stage('build') {
            steps {
                sh 'usermod -a -G docker jenkins'
                sh 'python3 ./manage.py'
            }
        }
    }
}
