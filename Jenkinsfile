pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        retry(count: 3) {
          sh 'wwwwwwwww'
        }

        echo 'Build Completed'
      }
    }

    stage('Test Stages') {
      parallel {
        stage('Test2') {
          steps {
            echo 'Running Test2'
          }
        }

        stage('Test1') {
          steps {
            echo 'Running Test1'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        input(message: 'Are you Ready to deploy', ok: 'Yes I\'m Sure')
        echo 'Deployment Completed'
        sh 'date'
      }
    }

    stage('Notify For new Build') {
      steps {
        echo 'Build Completed Suucessfully'
      }
    }

  }
}