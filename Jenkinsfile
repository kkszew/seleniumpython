pipeline {
    agent {
        docker { image 'python:3.10-slim' }
    }
    stages {
        stage ('Install'){
            steps{
                sh 'pip install -r requirements.txt'
            }
        }

        stage('Test'){
            steps{
               sh 'pytest tests/test_math_py'
            }
        }
    }
}