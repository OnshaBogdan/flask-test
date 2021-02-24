pipeline {
    agent { docker { image 'python:3.7.2' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                sh 'python -m pip install --user flask'
            }
        }
    }
}


