pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                script {
                   def centos = docker.image('centos')
                    centos.pull() // make sure we have the latest available from Docker Hub
                    centos.inside {
                          sh 'mkdir sharon_homo'
                          sh 'ls -l /'

                    } 
                }
             }
        }
        stage('Test') { 
            steps {
                sh 'echo shi2t' 
            }
        }
       
    }
}
