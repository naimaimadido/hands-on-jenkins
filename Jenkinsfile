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
            echo 'Testing Firefox ...'
          }
        }

        stage('Test Chrome') {
          steps {
            echo 'Testing Chrome...'
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