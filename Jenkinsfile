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

       stage ('GitCheckout'){
          steps {
             echo "Checking out from Git Repo";
             git "https://github.com/PrasanthNeocepts/JenkinsDemoIonic.git"
          }
       }
      stage('NPM Setup') {
      steps {
         bat 'npm install'
      }
      }

      stage('Publish iOS') {
      steps {
       echo "Publish iOS Action"
    }
   }

   stage('Publish Android') {
     steps {
    echo "Publish Android API Action"
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

