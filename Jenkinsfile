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
    stage('deploy') {
      steps {
        sh 'echo "deploy"'
      }
    }
  }
}