#!groovy
pipeline {
    agent any

    stages {
        stage('Build docker file') {
            steps   {
                sh "docker build -t project-image:B${BUILD_NUMBER} ."
            }
        }
    }
}
