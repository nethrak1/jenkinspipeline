pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'hello Dev stage'
      }
    }
    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'Test stage '
          }
        }
        stage('test-sub') {
          steps {
            echo 'test sub stage'
          }
        }
      }
    }
    stage('Prod') {
      steps {
        echo 'Prod stage'
      }
    }
  }
}