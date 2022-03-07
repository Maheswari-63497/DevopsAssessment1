pipeline {
  agent any
  tools {
    maven 'Maven' 
  }
  stages {
     stage("maven build"){
            mavenGoals="clean test"         
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
