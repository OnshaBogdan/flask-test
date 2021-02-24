pipeline {
    agent { docker { image 'python:3.7.2' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'

            }
        }
        stage('test') {
            steps {
                sh 'sudo python test.py'
            }
        }
    }
}


