pipeline {
    agent { docker { image 'python:3.7.2' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                sh 'sudo virtualenv .venv'
                sh 'sudo source .venv/bin/activate'
                sh 'sudo python -m pip install -r requirements.txt'
            }
        }
    }
}


