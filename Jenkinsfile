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
                bat 'npm install'
            }
        }
        stage('Run Application') {
            steps {
                bat 'node index.js'
            }
        }
    }
    post {
        always {
            echo 'Pipeline completed.'
        }
    }
}