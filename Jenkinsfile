pipeline {
    agent any
    stages {
        stage('Step 1') {
            steps {
                sh 'echo "Ping google.com"'
                sh 'ping google.com -c 5'
            }
        }
        stage('Step 2') {
            steps {
                sh 'echo "For loop"'
                sh '''
                    #!/bin/bash
                    for char in {f..s}
                    do
                        echo $char
                    done
                ''' 
            }
        }
        stage('Step 3') {
            steps {
                sh 'echo "curl apache"'
                sh 'curl 192.168.56.31:80'
            }
        }
    }
}
