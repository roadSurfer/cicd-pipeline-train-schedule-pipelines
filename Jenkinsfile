pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Running automated build'
        sh './gradlew build --no-deamon'
        archiveArtifacts artifact 'dist/trainSchedule.zip'
      }
    }
  }
}
