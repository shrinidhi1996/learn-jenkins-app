pipeline {
    agent {
        docker { image 'node:16-alpine' }
    }
    
    stages {
       
        stage('npm run') {
            steps {
                echo 'running the npm '
                sh '''
                    npm --version
                    npm start
                '''
            }
        }
    }
}
