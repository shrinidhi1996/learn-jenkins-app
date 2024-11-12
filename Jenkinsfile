pipeline {
    agent {
        docker { image 'node:18-alpine' }
    }
    
    stages {
       
        stage('npm run') {
            steps {
                echo 'running the npm '
                sh '''
                    npm --version
                    node --version
                    npm ci
                    npm run build
                    ls -l
                '''
            }
        }

        stage('npm test') {
            steps {
                sh '''
                    npm test
                    cd build
                    test -f index.html
                '''
            }
        } 
    }
}
