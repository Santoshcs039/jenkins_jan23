pipeline {
    agent {
        label 'slave2'
    }
    stages {
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