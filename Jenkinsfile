pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Compile the Java Code'
          }
        }

        stage('Test') {
          steps {
            echo 'Run Test Suite'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        input(message: 'Do you want to Deploy ?', id: 'Ok')
      }
    }

  }
  environment {
    appName = 'HelloWorld'
  }
}