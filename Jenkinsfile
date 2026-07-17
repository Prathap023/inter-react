pipeline {
    agent any
    
    triggers {
        cron('H/2 * * * *')
    }
    
    tools {
        nodejs 'node'
    }
    
    stages {
        stage('Checkout') {
            steps {
                git branch: 'master', url: 'https://github.com/Prathap023/inter-react.git'
            }
        }
        
        stage('Build') {
            steps {
                echo "Building the application..."
                sh 'npm install'
            }
        }
        
        stage('Run') {
            steps {
                echo "Running the application..."
                sh 'npm start &' 
            }
        }
    }
}
