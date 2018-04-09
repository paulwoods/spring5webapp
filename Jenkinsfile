pipeline {
  agent any
  stages {
    stage('init') {
      steps {
        bat 'maven3'
      }
    }
    stage('clean') {
      steps {
        bat 'mvn clean'
      }
    }
  }
}