pipeline {
  agent {
    docker {
      image 'node:10.13.0-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh '''npm config set registry https://registry.npm.taobao.org
npm install'''
      }
    }
  }
}