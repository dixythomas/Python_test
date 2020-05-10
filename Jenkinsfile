pipeline {
   agent any
   parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
     }
   stages {
      stage('Hello') {
         when{
            branch'master'
          }
         steps {
            echo "${env.BRANCH_NAME}"
            echo "${params.PERSON}"
            sh 'python frog_jump.py'
         }
      }
   }
}