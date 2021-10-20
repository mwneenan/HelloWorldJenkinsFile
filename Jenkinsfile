pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }

  }
  stages {
    stage('Build') {
      agent {
        docker {
          image 'mwneenan/morgantest:1.0'
          reuseNode true
        }

      }
      steps {
        sh 'pwd'
        sh 'ls'
        sh 'npm --version'
        sh 'cdk --version'
      }
    }

  }
}