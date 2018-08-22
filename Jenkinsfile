pipeline {
    agent any 
    stages {
        stage('Build') {
            steps {
                echo "Building.."
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
            }
        }
        stage('Deliver for development') {
            when {
                branch 'development' 
            }
            steps {
                echo "Deliver fo development.."
            }
        }
        stage('Deploy for production') {
            when {
                branch 'production'  
            }
            steps {
                echo "Deliver for production.."
            }
        }
    }
}
