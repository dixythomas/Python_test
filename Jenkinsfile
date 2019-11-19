pipeline {
    agent any
    options {
  checkoutToSubdirectory ''
}
    stages {
        stage('build') {
            steps {
                sh 'python frog_jump.py'
            }
        }
    }
}