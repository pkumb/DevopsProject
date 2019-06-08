#!groovy
pipeline {
    agent any

    stages {
        stage('Build docker file') {
            steps   {
                sh "docker build -t project-image:B${BUILD_NUMBER} ."
            }
        }
        stage('Docker run') {
            steps {
                sh "docker run -d -p 80:80 project-image:B${BUILD_NUMBER} "
            }
        }
    }
}
