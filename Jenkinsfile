pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/yogi9016/TravelMemory/'
            }
        }
        stage('Install') {
            steps {
                sh 'cd backend'
                sh 'npm install'
            }
        }
        stage('Build') {
            steps {
                sh 'cd backend'
                sh 'npm run build'
            }
        }
    }
}
