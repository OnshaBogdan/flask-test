pipeline {
    agent { docker { image 'python:3.8.2' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                sh 'python -m venv env'
                sh 'sudo python -m pip install --upgrade pip'
                sh 'sudo python -m pip install -r requirements.txt'
                sh 'python -m pip freeze'
                sh 'python app.py'
            }
        }
    }
}