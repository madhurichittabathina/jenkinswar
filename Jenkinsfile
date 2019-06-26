pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/Ajayvarma8142/jenkinswar.git', branch: 'master')
      }
    }
    stage('build') {
      steps {
        bat 'mvn clean install'
      }
    }
  }
}