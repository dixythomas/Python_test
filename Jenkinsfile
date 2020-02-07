pipeline {
   agent any

   stages {
      stage('Hello') {
input {
		string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
                }
            }
         steps {
            echo 'Hell ${PERSON}'
            sh 'python frog_jump.py'
         }
      }
   }