pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                script {
                   def centos = docker.image('centos')
                    centos.pull() // make sure we have the latest available from Docker Hub
                    centos.inside {
                          sh 'echo hostname >sharon'
                          sh 'cp ./sharon /'
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
