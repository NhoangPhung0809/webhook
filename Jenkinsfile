pipeline {
  agent { docker { image 'python:3.7.2' } }
  stages {
    stage('vui'){
      steps { sh 'sudo usermod -aG docker $USER'}
    }
    stage('build') {
      steps {
          sh 'pip install -r requirements.txt'
      }
    }
    stage('test') {
      steps {
        sh 'python manage.py'
      }   
    }
  }
}
