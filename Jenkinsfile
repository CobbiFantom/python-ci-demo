
pipeline {
    agent any

    stages {
        stage('Check Python') {
            steps {
                sh 'python3 --version'
                sh 'python3 -m venv --help'
            }
        }

        stage('Install dependencies and test') {
            steps {
                sh '''
                    .venv/bin/python -m pip install -r requirements.txt
                    .venv/bin/python -m pytest -v
                '''
            }
        }
    }
}
