pipeline {
  agent any
  stages {
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