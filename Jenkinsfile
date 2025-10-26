pipeline {
    agent any

    triggers {
        githubPush()   // Auto trigger when a push happens
    }

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/<your-username>/jenkins-python-demo.git'
            }
        }

        stage('Run Python Script') {
            steps {
                sh 'python3 hello.py'
            }
        }
    }
}
