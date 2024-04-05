pipeline {
  agent any

tools { nodejs "node"}

  stages {
    stage('Build') {
      steps {
        git "https://github.com/MarlonRoches/SoftwareLab4-2024.git"
        sh 'npm install'
        sn "npm start"
      }
    }
  }
}
