pipeline {
  agent any
  stages {
    stage('First') {
      steps {
        echo 'Hi, This is my first pipeline stage ${appName}'
      }
    }

  }
  environment {
    appName = 'HelloWorld'
  }
}