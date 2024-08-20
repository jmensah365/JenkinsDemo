pipeline {
    agent any //any agent that is availabe can run this

    stages{
        stage('Build Frontend'){
            steps{
                sh "echo Building Frontend"
                sh "cd jenkinsfrontend && npm install && npm run build"
            }
        }
    }
}
