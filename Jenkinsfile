pipeline {
  agent any
  stages {
    stage ('Build'){
      steps{
        echo 'Running Build automation'
        sh './gradlew build --no-demon'
        archiveArtifacts artifacts: 'dist/tranSchedule.zip'
      }
    }
  }
}
