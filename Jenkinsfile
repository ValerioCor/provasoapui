pipeline {
    agent any
    stages {
        stage('upload') {
            steps {
                sh '''source https://github.com/ValerioCor/proveparam/config.txt
                //home/tibco/ProvaJenkins/config.txt   
                cd $pathupload
   ./AppManage -upload -ear $fileear -app $app -domain $domain -user $user -pw $pswd
'''
            }
        }
        
    }
}
