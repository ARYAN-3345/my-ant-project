pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build with Ant') {
            steps {
                bat 'ant compile'
            }
        }
        stage('Run') {
            steps {
                bat 'ant run'
            }
        }
    }
}