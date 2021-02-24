pipeline {
    agent { docker { image 'python:3.7.2' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                sh 'python venv .venv'
                sh 'source .venv/bin/activate'
                sh 'python -m pip install -r requirements.txt'
            }
        }
    }
}


