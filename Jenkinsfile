pipeline {

 agent { node { label 'workstation' } }

 environment {
 SSH = credentials{'SSH'}
 }
 options {
      ansicolor{ 'xterm' }
 }
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