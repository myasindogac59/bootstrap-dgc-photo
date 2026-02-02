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
                sh 'docker --version'
            }
        }
        stage('Deploy') {
            when{
                branch 'main'
            }
            steps{
                echo 'deploy aşamasi'
            }
        }
    }
}