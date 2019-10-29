pipeline {
   agent any
      // environment {
      //    PATH='C:/Program Files/nodejs/'
      // }
   stages {
       stage ('Message'){
          steps {
            echo 'Running Successfully'
          }
       }
       stage ('JUnit') {
          steps {
             echo "JUnit passed successfully"
          }
       }

       stage ('Quality Gate') {
          steps {
             echo "Quality Gate passed successfully"
          }
       }

       stage ('Deploy'){
          steps {
             echo "Pass!"
          }
       }
      }

      post {
         always {
            echo 'This will always run'
         }
         success {
            echo 'This will run only if success!'
         }
         failure {
            echo 'This will run only if failed'
         }
         unstable {
            echo 'This will run only if the run was marked as unstable'
         }
         changed {
            echo 'This will run only if the changed'
         }
      }
}

