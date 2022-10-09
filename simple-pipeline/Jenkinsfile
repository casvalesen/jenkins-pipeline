pipeline { 
    agent any 
    environment {
        mainenv = "dev"
    }
    stages {
        stage('stage 1') {
            environment {
                subenv = "prod"
            }
            steps {
            
                echo "Hello world"
                echo BUILD_ID
                echo """inside stage 1: mainenv = ${mainenv}"""
                echo """inside stage 1: subenv = ${subenv}"""
                
            }
            
        }
        stage('stage 2'){
            environment {
            subenv = "prod"
            }
            steps {
                echo """sinde stage 2: mainenv = ${mainenv}"""
                echo """inside stage 2: subenv = ${subenv}"""

            }
        }
    }
    