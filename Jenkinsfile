pipeline {
  agent any

  stages {
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
  post {
    always {
      archiveArtifacts artifacts: 'build/**', allowEmptyArchive: true
    }
  }
}
