pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "hello world"'
      }
    }

    stage('Dev') {
      parallel {
        stage('Dev') {
          steps {
            echo 'Dev Stage'
          }
        }

        stage('QA') {
          steps {
            echo 'QA Environment'
          }
        }

      }
    }

    stage('PROD') {
      steps {
        echo 'PROD envt'
      }
    }

  }
}