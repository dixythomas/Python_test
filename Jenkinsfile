pipeline {
   agent any
   parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
     }
   stages {
      stage('Hello') {
        when{
          branch 'origin/master'
        }
         steps {
            echo env.BRANCH_NAME
            sh 'git branch'
            echo "${params.PERSON}"
            sh 'python frog_jump.py'
          }
      }
   }
}