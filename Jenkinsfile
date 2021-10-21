pipeline {
  agent {
    docker {
      image 'mwneenan/morgantest:2.0'
    }

  }
  stages {
    stage('Test') {
      steps {
        sh 'whoami'
        sh 'pwd'
        sh 'ls'
        sh 'npm --version'
        sh 'cdk --version'
        sh 'amplify --version'
      }
    }

  }
}
