pipeline {
    agent any
    stages {
        stage('pull image') {
            steps {
               sh "docker pull maven:3.9.4-eclipse-temurin-17-alpine"
            }
        }
        stage('run image') {
            steps {
                sh "docker run -d -p 9000:9000 maven:3.9.4-eclipse-temurin-17-alpine"
            }
        }
    }
}

