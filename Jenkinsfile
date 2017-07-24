pipeline {
    agent any
    stages {
        stage('upload') {
            steps {
                sh '''source /home/tibco/ProvaJenkins/config.txt   
                cd $pathupload
   ./AppManage -upload -ear $fileear -app $app -domain $domain -user $user -pw $pswd
'''
            }
        }
        
    }
}
