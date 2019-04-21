pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo '123456'
      }
    }
    stage('test') {
      steps {
        bat 'echo "test"'
      }
    }
  }
  post {
    always {
      archiveArtifacts(artifacts: '*.txt', fingerprint: true)

    }

  }
}