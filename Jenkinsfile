pipeline {
    agent any
    environment {
        TEST = "test value"
        TEST1 = "test value1"
    }
    stages {
        
        stage('Build') {
            environment {
                BUILD_NAME = "my_build"
            }
            
            steps{
                    sh '''
                    echo $TEST $BUILD_NAME
                    sleep 5
                '''
                }
         
        }
    
        stage('Test') {
        
            steps{
                script {
                    echo "${env.TEST}"
                
                }
            }


        }
    }
}