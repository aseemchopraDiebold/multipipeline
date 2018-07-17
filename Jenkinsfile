pipeline {
    agent any
    triggers { 
        pollSCM('* * * * *') 
    }
    stages {
        stage('Build') {
            parallel {
                stage('Build WebApp') {
                    steps {
                        echo "Hello 1"
                    }
                }
                stage('Build C++') {
                    steps {
                        echo "Hello 2"
                    }
                }
            }
        }        
    }
}