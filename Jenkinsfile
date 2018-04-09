pipeline {
  agent any
  stages {
    stage('Unit Tests') {
      stage('clean') {
        steps {
          bat 'maven3'
          bat 'mvn clean'
        }
      }
      stage('test') {
        steps {
          bat 'mvn test'
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
