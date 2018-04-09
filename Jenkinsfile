pipeline {
  agent any
  stages {
    stage('Unit Tests') {
      steps {
        sh 'gradlew test'
      }
    }
    stage('Package') {
      steps {
        sh 'gradlew bootJar'
      }
    }
  }
}