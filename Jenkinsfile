pipeline {
    agent any 
    stages {
        stage ('Docker Build') {
            steps {
                bat 'docker build -t react .'
            }
        }
        stage ('Docker Run') {
            steps {
                bat 'docker run -d --name react -p 80:80'
            }
        }
    }
}
