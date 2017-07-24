pipeline {
    agent any
    stages {
        stage('upload') {
            steps {
                sh '''source /home/tibco/ProvaJenkins/config.txt   
                cd $pathupload
   ./AppManage -upload -ear $fileear -app Prove -domain ProveJenkins -user $admin -pw $pswd
'''
            }
        }
        
    }
}
