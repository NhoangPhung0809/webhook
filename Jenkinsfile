pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage ('buid') {
            steps {
                sh 'python manage.py'
            }
        }
    }
}
