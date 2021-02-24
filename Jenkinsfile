pipeline {
    agent { docker { image 'python:3.7.2' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                sh 'python -m pip install virtualenv'
                sh 'virtualenv -p python .venv'
                sh 'source .venv/bin/activate'
                sh 'python -m pip install -r requirements.txt'
            }
        }
    }
}


