pipeline {
    agent { docker { image 'python:3.8.2' } }
    stages {
        stage('build') {
            steps {
                sh 'python -m pip install flask'
            }
        }
        stage('run') {
            steps {
                sh 'python app.py'
            }
        }
    }
}
}