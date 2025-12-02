pipeline {

    agent any

    tools {
        maven 'Maven3'
        jdk 'Java 21.0.7'
    }

    stages {

        stage('Clean') {
            steps {
                sh 'mvn clean'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn compile'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }

        stage('Package') {
            steps {
                sh 'mvn package'
            }
        }

    }
}
