pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            sh 'echo "start pipeline"'
          }
        }

        stage('stage 11') {
          steps {
            sh 'echo $formation'
          }
        }

      }
    }

    stage('stage 2') {
      steps {
        sh 'free -h'
      }
    }

  }
  environment {
    formation = 'plb'
  }
}