pipeline {
    agent any

    stages {
        stage('Test') {
            steps {
                sh 'python3 --version'
                sh 'python3 -m pip install pytest'
                sh 'python3 -m pytest -v'
            }
        }
    }
}