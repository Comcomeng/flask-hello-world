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
                sh 'pip install -r requirements.txt'
            }
        }

        stage('Run Flask App') {
            steps {
                sh 'python app.py & sleep 5'
                echo 'Flask app is running in the background...'
            }
        }
    }
}
