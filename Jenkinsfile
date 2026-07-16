pipeline{
    agent any
    stages{
        stage('Checkout'){
            steps{
                bat 'echo "Checking out the code..."'
                checkout scm
            }
        }
        stage('Build'){
            steps{
                bat 'echo "Building the application..."'
                bat 'npm install'
            }
        }
        stage('Run'){
            steps{
                bat 'echo "Running the application..."'
                bat 'npm start'
            }
        }
    }
}