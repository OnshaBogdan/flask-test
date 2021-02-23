pipeline {
    agent { docker { image 'python:3.8.2' } }
    stages {
        stage('build') {
            steps {
                sh 'python -m pip install --user flask'
            }
        }
        stage('run') {
            steps {
                sh 'python app.py'
            }
        }
    }
}