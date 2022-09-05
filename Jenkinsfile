pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'buliding'
            echo '"get the driver path of $(Chromrdriverpath)"'
          }
        }

        stage('test') {
          steps {
            echo 'testing the build'
          }
        }

      }
    }

    stage('deploy') {
      agent any
      steps {
        echo 'deploy to app'
        input(message: 'still do u want to deploy', id: 'ok')
      }
    }

  }
  environment {
    Chromrdriverpath = 'd:\\cent\\'
  }
}