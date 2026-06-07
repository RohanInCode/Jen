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
                bat 'docker run -d -p 8082:8080 myapp:1.0'
            }
        }
    }
}
