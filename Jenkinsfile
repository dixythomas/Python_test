pipeline {
    agent any
    checkout([$class: 'GitSCM', branches: [[name: '*/master']], 
    	doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/dixythomas/Python_test.git']]])
    stages {
        stage('build') {
            steps {
                sh 'python frog_jump.py'
            }
        }
    }
}