pipeline {
  agent {
    docker {
      image 'hello-world'
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