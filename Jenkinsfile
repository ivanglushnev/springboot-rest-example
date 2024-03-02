pipeline {
  agent any
  tools {
    maven '3.9.6'
  }
  stages {
    stage('checkout') {
      steps {
        git branch 'master', credentialsId: '67a42cfb-322c-482b-aa6b-930dd9bda981', url: 'https://github.com/ivanglushnev/springboot-rest-example.git'
      }
    }
    stage('build') {
    steps {
      sh 'mvn clean install'
    }
  }
}