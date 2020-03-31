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
        bat 'mvn clean compile'
      }
    }
    stage('Test') {
      steps {
        bat 'mvn test'
      }
  }
    stage('Deploy') {
      steps {
        bat 'mvn deploy'
      }
  }
}
