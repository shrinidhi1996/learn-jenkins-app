pipeline {
    agent {
      docker{
        image ''
      }
    }

    stages {
       stage('Git checkout') {
            steps {
                git branch: 'main', credentialsId: '77ccb602-8682-4ad7-8d94-2e7f2c8329eb', url: 'https://github.com/shrinidhi1996/learn-jenkins-app.git'
            }
        }
        stage('inside container') {
            steps {
                echo 'Hello World'
                sh 'pwd'
            }
        }
    }
}
