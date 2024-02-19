@Library('My-Jenkins-SharedLibrary')_

pipeline {
    agent any
    tools { 
        maven 'maven 3.9.6'
    }
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
