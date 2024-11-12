pipeline {
    agent any

    stages {
       
        stage('inside container') {
            steps {
                echo 'Hello World'
                sh 'pwd'
                sh 'ls -l'
            }
        }
    }
}
