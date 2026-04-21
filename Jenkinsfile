pipeline {
    agent{
        docker{
            image 'postman/newman'
            args '-u=root --entrypoint='
        }
    }
    
    stages {
        stage('Example 1') {
            steps {
                sh 'npm install'
            }
        }
        stage('Example 2') {
            steps {
                

                sh "newman run collection.json"
                    
                }    
            }
        
    }
}