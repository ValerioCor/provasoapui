pipeline {
    agent any
    stages {
        stage('upload') {
            steps {
                sh '''source /home/tibco/ProvaJenkins/config.txt   
                cd $pathdeploy
   ./AppManage -upload -ear $fileear -app Prove -domain ProveJenkins -user admin -pw admin
'''
            }
        }
        
    }
}
