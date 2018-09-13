pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "Building1.."'
        sleep 10
      }
    }
    stage('Test') {
      parallel {
        stage('Test1') {
          steps {
            sh 'echo "Test1"'
          }
        }
        stage('Test2') {
          steps {
            sh 'echo "Test2.."'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        sh 'echo "Deploy.."'
      }
    }
  }
}
