pipeline {
    agent {
        label 'node-1'
    }
    stages {
        stage('logging to ecr') {
            steps {
                aws ecr get-login-password --region eu-central-1 | docker login --username AWS --password-stdin 307854153830.dkr.ecr.eu-central-1.amazonaws.com
            }
        }
    }
}
