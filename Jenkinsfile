pipeline {
  agent any
  stages {
    stage('scm') {
      steps {
        git(url: 'https://github.com/Ajayvarma8142/jenkinswar.git', branch: 'master')
      }
    }
    stage('build') {
      steps {
        bat 'mvn install'
      }
    }
  }
}