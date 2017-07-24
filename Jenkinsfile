pipeline {
    agent any
    stages {
        stage('upload') {
            steps {
                sh '''cd $PATH
   ./AppManage -upload -ear /home/tibco/tibco/designer/5.10/ProvePoller.ear -app Prove -domain ProveJenkins -user admin -pw admin
'''
            }
        }
        
    }
}
