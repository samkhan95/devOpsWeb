@Library('My-Jenkins-SharedLibrary')_

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    java() // Call the 'java' method from the shared library
                }
            }
        }
        stage('Deploy') {
            steps {
                script {
                    react() // Call the 'react' method from the shared library
                }
            }
        }
    }
}
