pipeline {
  agent any
  stages {
    stage('stage one') {
      steps {
        parallel(
          "stage one": {
            sh 'cd /home/tibco/tibco/tra/5.10/bin'
            
          },
          "stage two": {
            sh './AppManage -stop -app Prove -domain ProveJenkins -user admin -pw admin'
            
          }
        )
      }
    }
  }
}
