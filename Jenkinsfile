pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git url: 'https://github.com/Prabhu308/vijay.git'
            }
        }
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Run Application') {
            steps {
                sh 'node index.js'
            }
        }
    }
    post {
        always {
            echo 'Pipeline completed.'
        }
    }
}