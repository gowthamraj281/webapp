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
            sleep 25
            mail(subject: 'temp', body: 'job', from: 'gowthamraj281@gmail.com', to: 'gowthamraj281@gmail.com', replyTo: 'gowthamraj281@gmail.com')
            sh 'vi temp.txt'
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