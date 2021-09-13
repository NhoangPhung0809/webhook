pipeline{
    agent any
    stages{
        stage("Build"){
            steps{
                chmod u+x './test.sh'
                sh './test.sh'
            }
        }
    }
}
