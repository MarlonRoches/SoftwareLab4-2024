pipeline {
  agent any

    tools { nodejs "node"}
    options {
        timeout(time: 15, unit: 'MINUTES') // Ajusta el tiempo de timeout global para la ejecución del pipeline
    }


  stages {
    stage('Clonar Repositorio'){
            // Pasos, autenticarnos, hacer fetch, etc
            steps{
                //Clonar el repositorio
        git "https://github.com/MarlonRoches/SoftwareLab4-2024.git"
            }
        }

    stage('Build') {
      steps {
        sh 'npm install'
      }
    }
  }
}
