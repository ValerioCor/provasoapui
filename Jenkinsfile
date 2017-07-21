 pipeline {
   agent any
   stages {
-    stage('build') {
+    stage('stage one') {
       steps {

+        parallel(
+          "stage one": {
+            sh 'pwd'
+            
+          },
+          "stage two": {
+            sh 'cd /home/tibco'
+            
+          }
+        )
       }
     }
   }
