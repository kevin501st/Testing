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
                sh 'mvn clean compile'
            }
        }
        stage('Testing') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                sh 'mvn install'
                sh 'java -jar ./target/testing-0.0.1-SNAPSHOT.jar'
            }
        }
    }
}
