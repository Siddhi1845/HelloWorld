pipeline {
    agent any

    stages {
        stage('clone') {
            steps {
                git branch: 'main', credentialsId: '7c273dc1-6cdc-4ffb-8f9e-770d5108ded1', url: 'https://github.com/Siddhi1845/HelloWorld.git'
            }
        }
        stage('Compile') {
            steps {
                bat 'javac hello.java'
            }
        }
        stage('Run') {
            steps {
                bat 'java Hello'
            }
        }
    }
}
