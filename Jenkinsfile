pipeline {
    agent any
    environment {
        PATH = "C:\\Windows\\System32;${env.PATH}"
    }
    stages {
        stage('Install Dependencies') {
            steps {
                bat 'pip install -r requirements.txt'
            }
        }
        stage('Run Flask App') {
            steps {
                bat 'python app.py'
            }
        }
    }
}
