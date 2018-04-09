pipeline {
  agent any
  stages {
    stage('Unit Tests') {
      parallel {
        stage('clean') {
          steps {
            bat 'mvn clean'
          }
        }
        stage('test') {
          steps {
            bat 'mvn test'
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