pipeline {
  agent 
  
    label "sonar"
  }
  stages {
    stage('Scan the code') {
      steps {
        withSonarQubeEnv('sonarqube6.7.7') {
          sh "mvn sonar:sonar"
        }
      }
    }
  }
}
