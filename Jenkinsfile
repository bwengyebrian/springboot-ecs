pipeline {
    agent any

    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo "./gradlew assemble"
            }
        }
        stage('Test') {
            steps {
                sh './gradlew test'
            }
        }
    }
}