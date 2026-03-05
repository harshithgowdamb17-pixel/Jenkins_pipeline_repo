pipeline {
    agent any

    options {
        ansiColor('xterm')
    }

    stages {

        stage('STAGE1') {
            steps {
                echo "\u001B[34mThis is the stage 1\u001B[0m"
                sh '''
                    sleep 5
                    echo -e "\e[32mThis is a linux command\e[0m"
                '''
            }
        }

        stage('Build') {
            steps {
                echo "\u001B[33mBuilding Java code\u001B[0m"
                sh '''
                    #!/bin/bash
                    sleep 5
                    echo -e "\e[31mBuild in progress...\e[0m"
                    echo -e "\e[32mBuild Successful\e[0m"
                '''
            }
        }

    }
}