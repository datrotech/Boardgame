pipeline {
    agent {
        label 'slave-1'
    }
    
    tools {
        maven 'maven3'
        jdk 'java17'
    }

    stages {
        stage('Compile') {
            steps {
                sh "mvn compile"
            }
        }
        stage('Test') {
            steps {
                sh "mvn test"
            }
        }
        stage('Build') {
            steps {
                sh "mvn package"
            }
        }
    }
}
