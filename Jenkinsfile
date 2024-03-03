pipeline {
    agent none
    environment {
        TEST = "test value"
        TEST1 = "test value1"
    }
    stages {
        
        stage('Build') {
            agent {
                label 'slave1'
            }

            steps{
                sh '''
                sleep 5
                echo $TEST $TEST1
                '''
                }
         
        }
    
        stage('Test') {
            agent any

            steps{
                sh '''
                    #!/bin/bash
                    ls
                    echo $TEST $TEST1
                    sleep 10
                '''
            }


        }
    }
}