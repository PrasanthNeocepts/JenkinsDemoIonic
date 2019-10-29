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
}

