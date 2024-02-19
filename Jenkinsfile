@Library('My-Jenkins-SharedLibrary')_

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                   java_build()
                }
            }
        }
        stage('Deploy') {
            steps {
                script {
                    deployDemo()
                }
            }
        }
    }
}
