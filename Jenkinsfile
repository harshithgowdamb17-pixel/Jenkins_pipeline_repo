pipeline{
    agent any
    stages {
        stage ('stage1'){
            steps{
                sh 'sleep 5'
                echo "This is the stage1"
            }
        }
        stage ('stage2'){
            steps{
                sh '''
                   #!/bin/bash
                   pwd
                   ls -lrt
                   sleep 5
                '''
                echo "This is the stage2"
            }
        }
        }
    }
