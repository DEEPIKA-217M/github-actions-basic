pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/DEEPIKA-217M/github-actions-basic.git'
            }
        }

        stage('Check Python') {
            steps {
                bat 'python --version'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat 'python -m pip install pytest'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'python -m pytest'
            }
        }
    }
}