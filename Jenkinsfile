pipeline {
  agent any
  stages {
    stage('Git Checkout') {
      steps {
        git url: "https://github.com/jeremy34270/game-of-life-1.git", branch: "master"
        }
    }
    stage('Build') {
      steps {
        sh 'mvn clean compile'
      }
    }
    stage('Test') {
      steps {
        sh 'mvn test'
      }
  }
}
