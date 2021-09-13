pipeline{
    agent any
    stages{
        stage("Build"){
            steps{
                sh "chmod +x -R ${env.WORKSPACE}"
                sh 'python manage.py'
             }
        }
    }
}
