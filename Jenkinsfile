pipeline {
    
    stages {
        agent {
        label 'slave1'
    }
        stage('Build') {

            steps{
                sh 'sleep 5'
                }
         
        }
    
        stage('Test') {
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