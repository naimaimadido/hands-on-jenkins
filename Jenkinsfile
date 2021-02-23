pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building ...'
      }
    }

    stage('Test') {
      parallel {
        stage('Test Firefox') {
          steps {
            echo 'Testing Firefox ...'
          }
        }

        stage('Test Chrome') {
          steps {
            echo 'Testing Chrome...'
            exit 1
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
