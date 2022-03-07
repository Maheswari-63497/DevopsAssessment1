pipeline {
  agent any
  tools {
    maven 'Maven' 
  }
  stages {
     stage("maven build"){
      /* steps {
          mavenGoals="clean test"    
       }*/
       
          withMaven {
      sh "mvn clean verify"
    } 
     }
  }
  

   /* stage ('Deploy') {
      steps {
        script {
          deploy adapters: [tomcat9(credentialsId: 'tomcat_credential', path: '', url: 'http://dayal-test.letspractice.tk:8081')], contextPath: '/pipeline', onFailure: false, war: 'webapp/target/*.war' 
        }
      }
    }*/
}
