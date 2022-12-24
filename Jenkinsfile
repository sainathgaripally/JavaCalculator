pipeline {
    agent {
        label 'node-1'
    }
    environment {
        AWS_REGION = '"eu-central-1"
    }
    stages {
        stage('logging to ecr') {
            steps {
                sh "aws ecr get-login-password --region eu-central-1 | docker login --username AWS --password-stdin 307854153830.dkr.ecr.${AWS_REGION}.amazonaws.com"
            }
        }
    }
}
