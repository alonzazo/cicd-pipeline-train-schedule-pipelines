pipeline {
  agent any
  stages {
    stage ('Build'){
      steps {
        echo 'Build'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
