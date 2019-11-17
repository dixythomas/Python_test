pipeline {
    agent { dockerfile true  }
    stages {
        stage('build') {
            steps {
                sh 'python frog_jump.py'
            }
        }
    }
}