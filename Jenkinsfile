@Library('My-Jenkins-SharedLibrary')_

pipeline {
    agent any
    tools { 
        maven 'maven'
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
                    deployDemo.deploy()
                }
            }
        }
    }
}
