pipeline{
    agent any
    stages{
        stage('Checkout'){
            checkout scm
        }
        stage('Build'){
            steps{
                sh 'echo "Building the application..."'
                sh 'npm install'
            }
        }
        stage('Run'){
            steps{
                sh 'echo "Running the application..."'
                sh 'npm start'
            }
        }
    }
}