pipeline {
    agent any //any agent that is availabe can run this

    stages{
        stage('Build Frontend'){
            steps{
                sh "echo Building Frontend"
                sh "cd jenkinsfrontend && npm install && npm run build"
            }
        }
        stage('Deploy Frontend'){
            steps{
                script{
                    withAWS(region: 'us-east-1', credentials: 'AWS_CREDENTIALS')
                    sh "aws sync jenkinsfrontend/dist s3://candy-inventory-management"
                }
            }
        }
    }
}
