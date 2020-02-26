pipeline {
  agent {
    docker {
      image 'hello-world'
      args 'run'
    }

  }
  stages {
    stage('docker') {
      steps {
        echo 'docker'
      }
    }
    stage('build') {
      steps {
        sh 'mvn clean package'
      }
    }
  }
}