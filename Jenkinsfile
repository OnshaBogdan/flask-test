pipeline {
    agent { docker { image 'python:3.7.2' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                sh 'apt-get install python-virtualenv -y'
                sh 'virtualenv -p python venv'
                sh 'source .venv/bin/activate'
                sh 'pip install -r requirements.txt'
            }
        }
    }
}


