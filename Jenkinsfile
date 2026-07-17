pipeline {
    agent any
    
    triggers {
        cron('H/2 * * * *')
    }
    
    stages {
        stage('Checkout') {
            steps {
                git branch: 'master', url: 'https://github.com/Prathap023/inter-react.git'
            }
        }
        
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        
        stage('Run') {
            steps {
                sh 'npm start &'
            }
        }
    }
    
    post {
        success {
            echo 'Pipeline executed successfully!'
        }
        failure {
            echo 'Pipeline failed. Please check the logs above.'
        }
    }
}
