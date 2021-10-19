pipeline {
    agent any
    stages {
        stage('Build') {
            agent {
                docker {
                    image 'mwneenan/morgantest:1.0'
                    // Run the container on the node specified at the top-level of the Pipeline, in the same workspace, rather than on a new node entirely:
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
