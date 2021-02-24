pipeline {
    agent { docker { image 'python:3.7.2' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                withEnv(["HOME=${env.WORKSPACE}"]) {
                    sh "pip install -r requirements.txt --user"
                }
            }
        }
        stage('run') {
            steps {
                sh 'python --version'
                withEnv(["HOME=${env.WORKSPACE}"]) {
                    sh "gunicorn -b 0.0.0.0:8000 app:app"
                }
            }
        }
    }
}


