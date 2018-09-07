pipeline {
  agent any
   stages {
     stage ('build') {
       steps{
       sh 'mvn build.xml -v'
       }
       }
       }
  post {
    always {
      archiveArtifacts artifacts:'dist/*.jar', fingerprint: true
    }
  }
  
}
       
