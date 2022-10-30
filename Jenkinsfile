pipeline {
  agent any
  stages {
    stage('clean') {
      parallel {
        stage('clean') {
          steps {
            echo 'hello'
          }
        }

        stage('error') {
          steps {
            sh 'echo "done"'
          }
        }

      }
    }

    stage('error') {
      steps {
        echo 'entered into step2'
      }
    }

  }
}