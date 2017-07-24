pipeline {
    agent any
    stages {
        stage('upload') {
            steps {
                sh '''cd /home/tibco/tibco/tra/5.10/bin/
   ../AppManage -upload -ear /home/tibco/tibco/designer/5.10/ProvePoller.ear -app Prove -domain ProveJenkins -user admin -pw admin
'''
            }
        }
        stage('deploy') {
             agent any {
label 'deploy'

       }
             steps {   
              
              sh '''cd /home/tibco/tibco/tra/5.10/bin/
   ../AppManage -deploy -ear /home/tibco/tibco/designer/5.10/ProvePoller.ear -app Prove -domain ProveJenkins -user admin -pw admin
'''
      
            }
        }
        stage('start') {
            agent none {
       label 'start'
            }
            steps {
          sh '''cd /home/tibco/tibco/tra/5.10/bin/
   ./AppManage -start -app Prove -domain ProveJenkins -user admin -pw admin'''
            }
        }
    }
}
