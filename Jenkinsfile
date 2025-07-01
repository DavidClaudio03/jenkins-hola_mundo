pipeline {
  agent any

  stages {
    stage('Clonar Repo') {
      steps {
        // Jenkins ya clona el repo automáticamente, este stage puede omitirse o dejar vacío
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
