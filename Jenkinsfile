pipeline {
    agent { dockerfile true  }
    stages {
        stage('build') {
            steps {
                sh 'docker build -t my-python-app .'
		sh 'docker run my-python-app'
            }
        }
    }
}