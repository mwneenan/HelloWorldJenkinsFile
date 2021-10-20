pipeline {
  agent {
    docker {
      image 'mwneenan/morgantest:1.0'
      args 'CDK_HOME=foo'
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