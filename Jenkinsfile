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

        stage('') {
          agent any
          steps {
            sh 'echo "done"'
          }
        }

      }
    }

    stage('') {
      steps {
        echo 'entered into step2'
      }
    }

  }
}