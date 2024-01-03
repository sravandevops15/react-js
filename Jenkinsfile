pipeline {
   agent {
     label 'build-server'
     }
     stages {
        stage ('Checkout') {
           steps  {
               checkout scm
             }
            }     
        stage ('Dependency-installation') {
              steps {
                    sh 'cd $WORKSPACE; npm install'

                }
            }
         stage ('Building') {
              steps {
                sh 'cd $WORKSPACE; npm run build'
           }
       } 
 }
     
}
