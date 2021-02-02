pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                script {
                   def centos = docker.image('centos')
                    centos.pull() // make sure we have the latest available from Docker Hub
                    centos.inside {
                          sh 'hostname'
                          sh 'whoami'
                          sh 'ls -l $(pwd)'

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
