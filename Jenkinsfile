pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/yogi9016/TravelMemory.git'
            }
        }
        stage('Install') {
            steps {
                sh 'cd backend; npm install'
            }
        }
        stage('Build') {
            steps {
                sh 'cd backend; npm run build'
            }
        }

    }
}
