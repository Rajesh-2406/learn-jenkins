pipeline {


    agent { node { label 'workstation' } }

    stages {
        stage('Hello1') {
            steps {
                echo 'Hello World'
            }
        }
    }
  post {
    always{
    sh 'echo post'
     }
   }
}