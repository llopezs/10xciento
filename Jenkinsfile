pipeline {
    agent any
    stages {
        stage('Clean') {
            withMaven(maven: 'mvn') {
            steps {
               script {
                sh "mvn clean"
               }
            }
        }

        stage('Compile') {
            withMaven(maven: 'mvn') {
            steps {
                script {
                sh "./mvn compile"
                }
            }
        }

        stage('Test') {
            withMaven(maven: 'mvn') {
            steps {
                script {
                sh "./mvn test"
                }
            }
        }
    }
}
