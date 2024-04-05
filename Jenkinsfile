pipeline {
  agent any

    tools { nodejs "node"}



  stages {
    stage('Clonar Repositorio'){
        steps{
        git "https://github.com/MarlonRoches/SoftwareLab4-2024.git"
        }
    }

    stage('install deps') {
      steps {
        sh 'npm install'
      }
    }
    stage('run dev') {
      steps {
        sh 'npm start'
      }
    }
  }
}
