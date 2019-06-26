pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/Ajayvarma8142/jenkinswar.git', branch: 'master')
      }
    }
    stage('build') {
      parallel {
        stage('build') {
          steps {
            bat 'mvn clean install'
          }
        }
        stage('sonar') {
          steps {
            bat 'mvn sonar:sonar'
          }
        }
      }
    }
    stage('clean') {
      steps {
        sh 'gradle clean'
      }
    }
  }
}