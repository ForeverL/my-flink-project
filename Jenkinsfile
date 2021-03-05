pipeline {
  agent any
  stages {
    stage('shell script') {
      parallel {
        stage('shell script') {
          steps {
            sh 'echo "test shell script"'
          }
        }

        stage('print message') {
          steps {
            echo 'print message'
          }
        }

        stage('sleep') {
          steps {
            sh '''echo "start to sleep"
sleep 5
echo "end to sleep"'''
          }
        }

      }
    }

    stage('') {
      steps {
        input(message: 'waiting for input', id: '1', ok: 'ok')
      }
    }

  }
}