pipeline {
   agent any
   parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
     }
   stages {
      stage('Hello') {
         when{
          env.GIT_BRANCH == 'origin/master'
         }
         steps {
            echo env.GIT_BRANCH
            echo "${params.PERSON}"
            sh 'python frog_jump.py'
          }
      }
   }
}