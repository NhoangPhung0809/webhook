pipeline {
    agent none
    stages (fix) {
            sh "sudo chown root:jenkins /run/docker.sock"
        }
    }
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage ('buid') {
            steps {
                sh 'python manage.py'
            }
        }
    }
}
