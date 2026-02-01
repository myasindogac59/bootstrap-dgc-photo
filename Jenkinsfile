pipeline {
    agent any
    environment {
        APP_NAME = 'myapp'
        ENV_NAME = 'dev'
    }
    stages{
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Test') {
            steps{
                sh 'whoami'
            }
        }
        stage('Build') {
            steps {
                echo "Build Aşaması"
                echo "${APP_NAME}"
                echo "${ENV_NAME}"
            }
        }
    }
}