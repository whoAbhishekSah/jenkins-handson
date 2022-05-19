pipeline {
    agent { docker { image 'python:3.10.1-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
        stage('run') {
            steps {
                echo 'print("hello world")' > run.py
                sh 'python run.py'
            }
        }
    }
}
