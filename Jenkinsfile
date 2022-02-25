pipeline {
  agent any
  stages {
    stage('Start') {
      steps {
        echo 'DevOps workflow start'
      }
    }

    stage('Fetch code') {
      steps {
        git(url: 'https://github.com/bill0871/public-toilet-map', branch: 'dev')
      }
    }

    stage('Build') {
      steps {
        sh 'mvn clean install'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy...'
      }
    }

  }
}