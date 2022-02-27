pipeline {
    agent any
    stages{
        stage ("first stage") {
            steps {
                sh "pwd"
                sh "ls"
                sh "echo test"
            }
        }

        stage("second stage") {
            steps {
               echo "hello world"
            }
        }
    }
}
