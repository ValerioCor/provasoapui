


pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                dir ('/home/tibco/tibco/tra/5.10/bin') 
                sh 'AppManage -stop -app Prove -domain ProveJenkins -user admin -pw admin'
            }
        }
    }
}


