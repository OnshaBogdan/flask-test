pipeline {
    agent { docker { image 'python:3.9' } }
    stages {
        stage('build') {
            steps {
                sh 'virtualenv .venv'
                sh 'source .venv/bin/activate'
                sh 'python -m pip install -r requirements.txt'
            }
        }
        stage('run') {
            steps {
                sh 'python app.py'
            }
        }
    }
}