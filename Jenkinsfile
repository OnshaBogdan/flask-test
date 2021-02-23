pipeline {
    agent { docker { image 'python:3.7.2' } }
    stages {
        stage('build') {
            steps {
                sh 'sudo virtualenv .venv'
                sh 'sudo source .venv/bin/activate'
                sh 'sudo python -m pip install -r requirements.txt'
            }
        }
        stage('test') {
            steps {
                sh 'sudo python test.py'
            }
        }
    }
}


