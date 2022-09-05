pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'buliding'
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
      }
    }

  }
}