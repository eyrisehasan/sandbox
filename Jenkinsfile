pipeline {
    agent any

    stages {
        stage('Checkout project') {
            steps {
                script {
                    git branch: "main",
                    url: 'https://github.com/eyrisehasan/sandbox.git'
                }
            }
        }
        stage('Hello') {
            steps {
                script {
                    sh 'python3 hello.py'
                }
            }
        }
        stage('Build') {
            steps {
                script {
                    sh 'python3 build.py'
                }
            }
        }
        stage('test') {
            steps {
                script {
                    sh 'python3 test.py'
                }
            }
        }
        stage('documentation') {
            steps {
                script {
                    sh 'python3 doc.py'
                }
            }
        }
    }
}
