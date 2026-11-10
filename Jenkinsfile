pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                checkout scm
                echo 'Code cloned successfully'
            }
        }

        stage('Compile') {
            steps {
                sh 'javac Hello.java'
            }
        }

        stage('Execute') {
            steps {
                sh 'java Hello'
            }
        }
    }
}
