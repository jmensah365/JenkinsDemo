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
        stage('Deploy'){
            steps{
                sh "echo Deploying stage 3"
            }
        }
    }
}
