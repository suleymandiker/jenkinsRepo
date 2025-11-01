pipeline {
    agent {
        docker {
            image 'python:3.11'
        }
    }
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/suleymandiker/jenkinsRepo.git'
            }
        }
        stage('Run Python Script') {
            steps {
                sh 'python main.py'
            }
        }
    }
}
