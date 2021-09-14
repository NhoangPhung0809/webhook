pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage ( 'ssh' ) {
            sh "sudo chown root:jenkins /run/docker.sock"
        }
        stage ('buid') {
            steps {
                sh 'python manage.py'
            }
        }
    }
}
