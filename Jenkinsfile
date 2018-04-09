pipeline {
  agent any
  stages {
    stage('Unit Tests') {
      parallel {
        stage('clean') {
          steps {
            sh 'mvn clean'
          }
        }
        stage('test') {
          steps {
            sh 'mvn test'
          }
        }
      }
    }
    stage('Package') {
      steps {
        sh 'gradlew bootJar'
      }
    }
  }
}