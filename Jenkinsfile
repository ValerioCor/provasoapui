pipeline {
  agent any
  stages {
    stage('stage one') {
      steps {
        parallel(
          "stage one": {
            sh '''/home/tibco/tibco/tra/5.10/bin/AppManage -stop -app Prove -domain ProveJenkins -user admin -pw admin'''
            
          }
        )
      }
    }
  }
}
