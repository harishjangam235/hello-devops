pipeline {
    agent any
    stages {
        stage('Checkout Code') {
    steps {
        git branch: 'main',
            credentialsId: 'github-creds',
            url: 'https://github.com/harishjangam235/hello-devops.git' 
            }
        }
        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }
    }
}
