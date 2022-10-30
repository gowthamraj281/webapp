pipeline {
  agent any
  stages {
    stage('package') {
      parallel {
        stage('package') {
          steps {
            sh 'echo "good evening"'
          }
        }

        stage('install') {
          steps {
            echo 'installed'
          }
        }

      }
    }

    stage('exit') {
      steps {
        echo 'pipeline succesfully done'
      }
    }

  }
}