pipeline {
   agent any
   parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
     }
   stages {
      stage('Hello') {
         steps {
            echo "${params.PERSON}"
            sh 'python frog_jump.py'
         }
         stage('new') {
         steps {
          if (branch == "origin/new_code"):
          {
            echo "${params.PERSON}"
            sh 'python frog_jump.py'
          }
         }
      }
   }
}