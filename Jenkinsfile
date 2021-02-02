pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                   def maven = docker.image('maven:latest')
                    maven.pull() // make sure we have the latest available from Docker Hub
                    maven.inside {
                      sh 'whoami'
                    } 
             }
        }
        stage('Test') { 
            steps {
                sh 'echo shit' 
            }
        }
       
    }
}
