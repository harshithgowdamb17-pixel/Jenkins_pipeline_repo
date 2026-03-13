pipeline {

    agent none

    stages {

        stage('Check Branch') {
            agent any
            steps {
                echo "Branch detected: ${env.BRANCH_NAME}"
                echo "Git branch: ${env.GIT_BRANCH}"
            }
        }

        stage('STAGE1 When branch harsha_banch01') {
            agent { label 'slave1' }
            when {
                branch 'harsha_banch01'
            }
            steps {
                echo "Running Stage1 for harsha_banch01"

                sh '''
                pwd
                ls -lrt
                sleep 5
                '''
            }
        }

        stage('STAGE2 When branch main') {
            agent { label 'slave2' }
            when {
                branch 'main'
            }
            steps {
                echo "Running Stage2 for main"

                sh '''
                pwd
                ls -lrt
                sleep 5
                '''
            }
        }

    }
}