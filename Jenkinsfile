pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git "https://github.com/Vishal3904/ci-node-app1.git"
            }
        }
        stage('Install') {
            steps {
                bat 'npm install'
            }
        }
        stage('Run App') {
            steps {
                bat 'node app.js'
            }
        }

        stage('Test') {
            steps {
                bat 'npm test'
            }
        }
    }
}