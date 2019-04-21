pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo '123456'
      }
    }
    stage('test') {
      parallel {
        stage('test') {
          steps {
            bat 'echo "test"'
          }
        }
        stage('test_2') {
          steps {
            bat 'echo "test_2"'
          }
        }
      }
    }
  }
  post {
    always {
      archiveArtifacts(artifacts: '*.txt', fingerprint: true)

    }

  }
}