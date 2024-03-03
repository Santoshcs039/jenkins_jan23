pipeline {
    agent any
    
    parameters {
        string(name: 'PARAM_STRING', defaultValue: 'input_param', description: 'This is string parameter')
        text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')
        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')
        choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')
        password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
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