pipeline {
    agent any
    stages {
        stage('upload') {
            steps {
                sh '''source proveparam/config.txt 
                //home/tibco/ProvaJenkins/config.txt   
                 proveparam/config.txt 
                cd $pathupload
   ./AppManage -upload -ear $fileear -app $app -domain $domain -user $user -pw $pswd
'''
            }
        }
        
    }
}
