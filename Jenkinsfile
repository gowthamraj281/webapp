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

        stage('update') {
          steps {
            sleep(time: 25, unit: 'NANOSECONDS')
            sh '''touch temp.txt
'''
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