pipeline {
   agent any
   parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
     }
   stages {
      stage('Hello') {
         when{
            anyOf{
              expression{env.BRANCH_NAME == "new_code"};
              branch 'master'
            }
          }
         steps {
            echo "${params.PERSON}"
            sh 'python frog_jump.py'
         }
      }
   }
}