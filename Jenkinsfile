pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                echo 'Building the application...'
            }
        }
        stage('Test'){
            steps{
                bat 'docker build -t myapp:1.0 .'
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deploying the application...'
            }
        }
    }
}
