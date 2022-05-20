pipeline{
  agent any
  stages{
    stage('validate'){
       steps{
         sh 'mvn validate'
       }
    }
    stage('build'){
       steps{
         echo 'Project is building'
       }
    }
    stage('test'){
       steps{
         echo 'Project is testing'
       }
    }
    stage('deploy'){
       steps{
         echo 'Project is deploying'
       }
    }
  }
}

