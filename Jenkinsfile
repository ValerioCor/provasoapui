pipeline {
    agent any
    stages {
        stage('upload') {
            steps {
                sh '''source <config.txt>
                        echo $pathdeploy
   ./AppManage -upload -ear /home/tibco/tibco/designer/5.10/ProvePoller.ear -app Prove -domain ProveJenkins -user admin -pw admin
'''
            }
        }
        
    }
}
