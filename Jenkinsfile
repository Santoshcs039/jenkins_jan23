pipeline {
    agent any
    
    parameters {
        string(name: 'PARAM_STRING', defaultValue: 'input_param', description: 'This is string parameter')
    }
    stages {
        
        stage('Build') {
                       
            steps{
                    sh '''
                    echo $PARAM_STRING
                    sleep 5
                '''
                }
         
        }
    
        stage('Test') {
        
            steps{
                script {
                    echo "${params.PARAM_STRING}"
                
                }
            }


        }
    }
}