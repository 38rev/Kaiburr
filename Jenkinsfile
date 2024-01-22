pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                script{
                     sh 'npm install'
                }
            }
        }
        stage('Docker Build Images') {
            steps {
                script {
                    sh 'docker build -t rev/CICD:v1 .'
                    sh 'docker images'
                }
            }
        }
    }
}
