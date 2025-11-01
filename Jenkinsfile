pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/suleymandiker/jenkinsRepo.git'
            }
        }
        stage('Run Python Script') {
            steps {
                sh 'python3 main.py'
            }
        }
    }
}
