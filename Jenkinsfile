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
                    def demoVar = 'Hello World'
                    deployDemo.deploy(demoVar)
                }
            }
        }
    }
}
