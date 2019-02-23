pipeline {
    agent {
        docker {
            image 'golang:1.12' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'go run app.go' 
            }
        }
    }
}