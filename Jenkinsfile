pipeline{
    agent any
    stages{
        stage("Build"){
            steps{
                chmod -R 777 ./test
                sh './test.sh'
            }
        }
    }
}
