pipeline{
    agent { docker { image 'python:3.5.1' } }
    stages{
        stage("Build"){
            steps{
                sh "chmod +x -R ${env.WORKSPACE}"
                sh 'python manage.py'
             }
        }
    }
}
