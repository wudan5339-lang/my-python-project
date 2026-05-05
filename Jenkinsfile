pipeline{
    agent any
    stages {

        stage('Install Dependencies'){
            steps {
                sh 'pip3 install -r requirement.txt'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'pytest'
            }
        }

        stage('Run App') {
            steps {
                sh 'python3 main.py'
            }
        }
    }
}