pipeline {
  agent any
  stages {
    stage('first stage') {
      parallel {
        stage('first stage') {
          steps {
            sh 'pwd'
            sh 'ls'
            sh 'echo test'
          }
        }

        stage('first stage 1') {
          steps {
            sleep 5
          }
        }

        stage('first stage 2') {
          steps {
            node(label: 'demo')
          }
        }

      }
    }

    stage('second stage') {
      steps {
        echo 'hello world'
      }
    }

  }
}