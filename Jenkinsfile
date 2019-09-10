pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/madhurichittabathina/jenkinswar.git', branch: 'master')
      }
    }
    stage('build') {
      steps {
        bat 'mvn install'
      }
    }
    stage('sonarqube') {
      steps {
        bat 'mvn sonar:sonar'
      }
    }
    stage('deploy') {
      steps {
        bat 'xcopy "'
      }
    }
  }
}