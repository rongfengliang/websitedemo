pipeline {
  agent any
  stages {
    stage('maven build') {
      parallel {
        stage('maven build') {
          steps {
            sh 'echo "maven build app"'
          }
        }
        stage('npm install') {
          steps {
            sh 'echo "npm install"'
          }
        }
      }
    }
    stage('Test') {
            steps {
                sh 'run test'
            }
     }
    stage('deploy') {
      steps {
        sh 'echo "deploy"'
      }
    }
  }
}
