pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/Comcomeng/flask-hello-world'
            }
        }

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
