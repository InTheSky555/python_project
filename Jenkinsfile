pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent none
            steps {
                echo '123456' 
                archiveArtifacts artifacts: '*.txt', fingerprint: true
            }
        }
    }
}
