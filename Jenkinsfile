pipeline {
    agent any 
    stages {
        stage('Build') { 
            agent none
            steps {
                echo '123456' 
            }
        }
    }
    post {
        always {
            archive '*.txt'
        }
    }
}
