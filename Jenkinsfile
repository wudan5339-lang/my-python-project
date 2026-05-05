pipeline{
    agent any
    stages {
        stage('Checkout'){
            steps {
                git  'https://github.com/wudan5339-lang/my-python-project.git/'
            }
        }

        stage('Install Dependencies'){
            steps {
                sh 'pip3 install -r requirements.txt'
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