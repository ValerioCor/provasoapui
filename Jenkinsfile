


pipeline {
    agent any
    stages {
        stage('build') {
            steps {
            sh '''cd /home/tibco/tibco/tra/5.10/bin
                 ./AppManage -stop -app Prove -domain ProveJenkins -user admin -pw admin'''
            }
        }
    }
}


