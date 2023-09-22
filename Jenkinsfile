pipeline {

 agent { node { label 'workstation' } }

 environment {
       SSH = credentials('SSH')
 }

 triggers { pollSCM('H/2 * * *') }

    stages {
        stage('Hello1') {
            steps {
                echo 'Hello World'
                sh 'env'
            }
        }
    }
  post {
    always{
    sh 'echo post'
     }
   }
}