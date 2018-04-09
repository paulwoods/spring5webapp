pipeline {
  agent any
  stages {
    stage('tools') {
      steps {
        bat '''maven3
        bat mvn clean
        bat mvn test'''
      }
    }
  }
}
