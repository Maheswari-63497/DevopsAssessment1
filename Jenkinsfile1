pipeline {
  agent any
  tools {
    maven 'Maven' 
  }
  stages {
     stage("maven build"){
 steps {
        bat 'mvn clean package'
             /* mavenGoals="clean test"   
             withMaven {
      sh "mvn clean verify"
    } 
    */
       }
       
          
     }
  }
  

 /*stage ('Deploy') {
      steps {
        script {
          deploy adapters: [tomcat9(credentialsId: 'tomcat_credential', path: '', url: 'http://dayal-test.letspractice.tk:8081')], contextPath: '/pipeline', onFailure: false, war: 'webapp/target/*.war' 
        }
      }
    }*/
}

/*pipeline {
  agent any
  tools {
    maven "Maven"
  }
  stages {
    stage('Initialize'){
  steps{
      echo "PATH = ${M2_HOME}/bin:${PATH}"
      echo "M2_HOME = /opt/maven"
    }
  }
stage('Build') {
    steps {
      dir("/var/lib/jenkins/workspace/demopipelinetask/my-app") {
      sh 'mvn -B -DskipTests clean package'
      }
    }
  }
}
post {
  always {
    junit(
      allowEmptyResults: true,
     
      )
    }
  }
}*/
