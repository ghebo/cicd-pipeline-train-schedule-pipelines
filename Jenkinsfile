pipeline {
  agent any
  stages {
    stage ('build'){
      steps {
        echo "Running build step"
        sh "./gradlew build --no-daemon"
        archiveArtifacts "dist/trainSchedule.zip"
      }
    }
  }
}
