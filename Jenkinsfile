pipeline{
    agent any
    stages{
        stage("Build"){
            steps{
                sh "chmod +x -R ${env.WORKSPACE}"
                sh './test.sh'
             }
        }
    }
}
