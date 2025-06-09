pipeline {
    agent any

    stages {
        stage('w/o docker') {
            steps {
                sh 'echo "Xin chao Bao dep trai"'
            }
        }
        stage('w docker') {
            agent{
                docker{
                    image 'node:18-alpine'
                }
            }
            steps {
                sh 'echo "Xin chao Bao dep trai"'
                sh 'npm --version'
            }
        }
    }
}
