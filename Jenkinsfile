pipeline {
    agent none
    stages {
        
        stage('Build') {
            agent {
                label 'slave1'
            }

            steps{
                sh 'sleep 5'
                }
         
        }
    
        stage('Test') {
            agent {
                label 'slave2'
            }
            steps{
                sh '''
                    #!/bin/bash
                    ls
                    pwd
                    uptime
                    sleep 10
                '''
            }


        }
    }
}