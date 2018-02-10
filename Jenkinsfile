pipeline {
   agent {
       docker 'maven:3-alpine'
   }
   tools {
       maven 'vova'
   }
   stages {
      stage('load') {
         steps {
             git 'https://github.com/koltysh/Maven.git'
         }
      }
      stage('pack') {
           steps {
             sh "mvn package"
          }
       }
   }
}
