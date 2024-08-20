pipeline {
    agent any //any agent that is availabe can run this

    stages{
        stage('Build'){
            steps{
                sh "echo Building stage 1"
            }
        }
        stage('Test'){
            steps{
                sh "echo Testing stage 2"
            }
        }
        stage('Test GitHub Webhooks'){
            steps{
                sh "echo It works"
            }
        }
        stage('Deploy'){
            steps{
                sh "echo Deploying stage 3"
            }
        }
    }
}
