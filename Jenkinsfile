pipeline {
    agent { docker { image 'python:3.7.2' } }
    stages {
        stage('build') {
            steps {
                sh 'virtualenv .venv'
                sh 'source .venv/bin/activate'
                sh 'python -m pip install -r requirements.txt'
            }
        }
        stage('test') {
            steps {
                sh 'python test.py'
            }
        }
    }
}


