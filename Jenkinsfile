pipeline {
    agent any

    environment {
        // Kalau perlu variabel, taruh di sini
    }

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

        stage('Run App or Test') {
            steps {
                // Jalankan script Python atau test-nya
                sh 'python app.py'
            }
        }
    }
}
