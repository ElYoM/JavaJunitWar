pipeline {
  agent any
  stages {
    stage('prepare') {
      agent any
      steps {
        git(url: 'https://github.com/ElYoM/JavaJunitWar2.git', branch: 'master')
      }
    }

    stage('build') {
      steps {
        sh 'mvn clean install'
      }
    }

  }
}