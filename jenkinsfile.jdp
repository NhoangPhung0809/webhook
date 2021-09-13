pipeline {
    agent any
    stages {
        stages('Build') {
            steps {
                py manage.py runserver
            }
        }

    }
}
