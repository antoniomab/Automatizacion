pipeline {
  agent any
  stages {
    stage('Log tool version') {
      steps {
        sh '''docker version
systeminfo'''
      }
    }

    stage('validate file') {
      steps {
        fileExists 'index.html'
      }
    }

    stage('generate file') {
      steps {
        writeFile(file: 'status.txt', text: 'Este pipeline funciona')
      }
    }

  }
}