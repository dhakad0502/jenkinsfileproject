

pipeline {
    agent any
    
   
    
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('build') {
            steps {
                echo 'Hello World you are going to build '
                echo "Hello World you are going to build WITH VERSION ${NEW_VERSION}"
            }
        }
        stage('Test') {
            
            when{
                expression{
                params.executeTeste
                }
            }
            steps {
                echo 'Hello World you are going to test '
            }
        }
        stage('Deploy') {
            steps {
                echo 'Hello World you are going to Deploy '
            }
        }
    }
}
