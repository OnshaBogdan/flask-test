pipeline {
    agent { docker { image 'python:3.7.2' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                withPythonEnv('python') {
                    sh 'pip install -r requirements.txt'
                }
            }
        }
    }
}


