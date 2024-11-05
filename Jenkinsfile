pipeline {
  agent any
  stages {
    stage('BUILD') {
      steps {
        echo 'This is a Build stage'
        sh '''
        sleep 5
            exit 0
       '''
      }
    }

    stage('TEST') {
      steps {
        echo 'This is a Test stage'
        sh 'sleep 5'
      }
    }

    stage('DEPLOY') {
      steps {
        echo 'This is a Deploy stage'
        sh 'sleep 5'
      }
    }
  }
}

