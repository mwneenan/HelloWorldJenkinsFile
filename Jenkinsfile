pipeline {
  agent {
    docker {
      image 'mwneenan/morgantest:2.0'
    }

  }
  stages {
    stage('Test') {
      steps {
        sh 'npm --version'
        sh 'cdk --version'
        sh 'amplify --version'
      }
    }

  }
}
