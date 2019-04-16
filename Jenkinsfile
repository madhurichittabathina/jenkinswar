pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git 'https://github.com/Ajayvarma8142/jenkinswar.git'
      }
    }
    stage('build') {
      steps {
        bat 'mvn install'
      }
    }
  }
}