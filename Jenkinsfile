pipeline {
  agent any
  stages {
    stage('Maven Build') {
      steps {
        echo 'First stage'
      }
    }
    stage('Stage 2') {
      steps {
        bat 'echo "Windows command"'
      }
    }
    stage('stage3') {
      parallel {
        stage('stage3') {
          steps {
            echo 'Printitng'
          }
        }
        stage('Stage4') {
          steps {
            cleanWs(cleanWhenSuccess: true)
          }
        }
      }
    }
  }
}