#!groovy
pipeline {
    agent any

    stages {
        stage('Build docker file') {
            steps   {
                sh "docker build -t project-image:ver1 ."
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
