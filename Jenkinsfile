pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running Build Stage'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
