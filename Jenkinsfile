pipeline {
    agent any 
    stages {
        stage ('Docker Build') {
            steps {
                bat 'docker build -t react .'
            }
        }
        stage ('rm perivious con') {
            steps {
                bat 'docker rm -f react || exit /b 0'
            }
        }
        stage ('Docker Run') {
            steps {
                bat 'docker run -d --name react -p 80:80 react'
            }
        }
    }
}
