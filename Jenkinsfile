pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git(url: 'https://github.com/deyvisrf/google-test-example.git', branch: 'master')
      }
    }
    stage('Install gems') {
      steps {
        sh '''cucumber
'''
      }
    }
    stage('Test UI') {
      steps {
        sh 'cucumber'
      }
    }
  }
}