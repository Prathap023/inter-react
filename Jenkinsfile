pipeline {
    agent any
    
    tools {
        git 'git' 
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Prathap023/inter-react.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'npm install'
            }
        }
        stage('Run') {
            steps {
                echo 'Running...'
            }
        }
    }
}
