pipeline {
  agent any
  tools {
    nodejs 'node'  // Replace with actual name or 'node'
  }
  stages {
    stage('Clone') {
      steps {
        cleanWs()
        git branch: 'main',
          url: 'https://github.com/sonarQube-prueba-eabmodel/pruebaSonarQ.git'
      }
    }
    stage('Ls prueba de archivos') {
      steps {
        sh 'ls'
      }
    }
    stage('Instalacion de dependencias carlos') {
      steps {
        nodejs('node') {
            sh '''npm --version'''
        }
      }
    }
  }
}
