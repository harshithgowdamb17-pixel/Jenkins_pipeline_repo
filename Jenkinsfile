pipeline {
    agent any

    options {
        ansiColor('xterm')
    }

    stages {

        stage('STAGE1') {
            steps {
                sh '''
                    echo -e "\\033[34mThis is the stage 1\\033[0m"
                    sleep 5
                    echo -e "\\033[32mThis is a linux command\\033[0m"
                '''
            }
        }

        stage('Build') {
            steps {
                sh '''
                    echo -e "\\033[33mBuilding Java code\\033[0m"
                    sleep 5
                    echo -e "\\033[31mBuild in progress...\\033[0m"
                    echo -e "\\033[32mBuild Successful\\033[0m"
                '''
            }
        }

    }
}