pipeline{
    agent any
    stages{
        stage('Checkout'){
            steps{
                sh 'echo "Checking out the code..."'
                checkout scm
            }
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
