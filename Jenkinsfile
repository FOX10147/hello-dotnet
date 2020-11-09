pipeline {
    agent none
    stages {
        stage('build') {
            agent any
            steps {
                 bat "dotnet build --configuration Release"
            }
        }
        stage('sonarqube') {
            agent any
            steps {
                sh 'echo sonarqube stage'
            }
        }
        stage('docker build') {
            agent any
            steps {
                sh 'echo docker build stage'
            }
        }
        stage('docker push') {
            agent any
            steps {
                sh 'echo docker push stage'
            }
        }
        stage('app deploy') {
            agent any
            steps {
                sh 'echo app deploy stage'
            }
        }
    }
}