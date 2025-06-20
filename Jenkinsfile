pipeline {
  agent any
  environment {
    HOME = "/home/anisa"
    MINIKUBE_HOME = "/home/anisa"
  }
  stages {
    stage('Clone') {
      steps {
        git branch: 'main', url: 'https://github.com/Anisyaaaaa/company-profile'
      }
    }
    stage('Build Docker Image') {
      steps {
        sh 'docker build -t company-profile:latest .'
      }
    }
    stage('Load to Minikube') {
      steps {
        sh 'minikube image load company-profile:latest'
      }
    }
    stage('Deploy to Kubernetes') {
      steps {
        sh '''
          kubectl apply -f k8s/deployment.yaml
          kubectl apply -f k8s/service.yaml
          kubectl apply -f k8s/ingress.yaml
        '''
      }
    }
  }
}
