pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                bat 'javac HelloWorld.java'
            }
        }

        stage('Test') {
            steps {
                bat 'java Hello World'
            }
        }

        stage('Archive') {
            steps {
archive Artifacts artifacts: '*.class', fingerprint: true
            }
        }
    }
}
