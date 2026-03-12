pipeline {
     agent none
   // options {
    //     ansiColor('xterm')
    //     disableConcurrentBuilds(abortPrevious: true)
    //     buildDiscarder(logRotator(numToKeepStr: '2'))
    //     disableResume()
    //     timeout(time: 1, unit: 'MINUTES')
    //     // retry(2)
    // }

    stages {

        stage('STAGE1 When branch harsha_banch01') {
            agent { label 'slave1' }
            when {
                branch 'harsha_banch01'
            }
            steps {
                echo "This is stage1 running"
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
                branch 'master/main'
            }
            steps {
                echo "This is stage2 running"
                sh ''' 
                    pwd
                    ls -lrt
                    sleep 5
                 '''
            }
        }

    }
}