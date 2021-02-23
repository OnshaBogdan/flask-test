pipeline {
    agent { docker { image 'python:3.8.2' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                sh 'pip3 install --upgrade pip'
                sh 'pip3 install -r requirements.txt'
                sh 'pip3 freeze'
                sh 'python app.py'
            }
        }
    }
}