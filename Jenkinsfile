pipeline {
    agent { docker { image 'python:3.10.1-alpine' } }
    stages {
        parallel{
            stage('build') {
                steps {
                    sh 'python --version'
                }
        }
            stage('run') {
                steps {
                    sh 'python run.py'
                }
            }
        }
    }
}
