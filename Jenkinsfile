pipeline {
  agent any
   stages {
     stage ('build') {
       steps{
       sh 'mvn build'
       }
       }
       }
  post {
    always {
      archiveArtifacts artifacts:'dist/*.jar', fingerprint: true
    }
  }
  
}
       
