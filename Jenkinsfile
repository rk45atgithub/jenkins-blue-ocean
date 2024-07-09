pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        echo 'start'
      }
    }

    stage('in progress') {
      parallel {
        stage('in progress') {
          steps {
            echo 'in progress'
            sleep 5
            sh '''date
pwd
'''
          }
        }

        stage('parallel') {
          steps {
            echo 'running parallel stage'
          }
        }

      }
    }

    stage('end') {
      steps {
        echo 'end'
      }
    }

  }
}