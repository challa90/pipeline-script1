pipeline {
  agent any
  tools {
    maven 'Maven 3.6'
    jdk 'JDK1.8'
  }
  stages {
    stage('Checkout') {
      steps {
        checkout scm
      }
    }
   
    stage('Clean') {
      steps {
        bat "mvn clean"
      }
    }
    
    stage('Package') {
      steps {
        bat "mvn package"
      }
    }
  }
}
