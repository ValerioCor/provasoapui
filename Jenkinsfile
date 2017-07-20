


pipeline {
    agent any
    stages {
        stage('build') {
            steps {
            
                sh './AppManage -stop -app Prove -domain ProveJenkins -user admin -pw admin -binding 192.172.2.51:8082'
            }
        }
    }
}


