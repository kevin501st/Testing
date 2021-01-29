pipeline {
    agent any

    tools {
     maven 'Maven'
    }

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World Testing Testing 1 2 3'
            }
        }
        stage('Build') {
            steps {
                sh './mvnw clean compile'
            }
        }
        stage('Testing') {
            steps {
                sh './mvnw test'
            }
        }
        stage('Deploy') {
            steps {
                sh './mvnw deploy'
            }
        }
    }
}
