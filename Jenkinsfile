pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building ...'
      }
    }

    stage('Test Firefox') {
      parallel {
        stage('Test Firefox') {
          steps {
            sh 'echo \'Test Firefox\''
          }
        }

        stage('Test Chrome') {
          steps {
            sh 'echo \'Test Chrome\''
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying ...'
      }
    }

  }
}