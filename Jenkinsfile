pipeline {
    agent any
    stages {
        stage('Clean') {
            steps {
               script {
                sh "mvn clean"
               }
            }
        }

        stage('Compile') {
            steps {
                script {
                sh "mvnw compile"
                }
            }
        }

        stage('Test') {
            steps {
                script {
                sh "./mvnw test"
                }
            }
        }
    }
}
