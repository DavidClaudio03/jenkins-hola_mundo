pipeline {
  agent any

  stages {
    stage('Clonar Repo') {
      steps {
         git 'https://github.com/DavidClaudio03/jenkins-hola_mundo.git'
      }
    }
    stage('Instalar dependencias') {
      steps {
        sh 'npm install'
      }
    }
    stage('Build') {
      steps {
        sh 'npm run build'
      }
    }
  }
}
