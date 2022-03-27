

pipeline {
    agent any
    
    parameters{
        choice(name:'version',choices:['1.0.0.0','1.0.1.0','1.1.0.0'], description:"")
        booleanparam(name:executeTeste,defaultvalue=true,description='')
    
    
    }
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
