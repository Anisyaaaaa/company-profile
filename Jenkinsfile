pipeline {
  agent any
  stages {
    stage('Clone') {
      steps {
        git 'https://github.com/Anisyaaaaa/company-profile'
      }
    }
    stage('Build Docker Image') {
      steps {
        sh 'docker build -t project-final13:latest .'
      }
    }
    stage('Push to Minikube (optional registry)' {
      steps {
        sh 'minikube image load project-final13:latest'
      }
    }
    stage('Deploy to K8s') {
      steps {
        sh 'kubectl apply -f k8s/'
      }
    }
  }
}
