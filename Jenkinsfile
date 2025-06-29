pipeline {
    agent any

    environment {
        PATH = "C:/Program Files/Git/cmd;${env.PATH}"
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Dev00-1/my-hello-app.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
                // Example: Run Python script
                sh 'python3 hello.py'
            }
        }
    }
}
