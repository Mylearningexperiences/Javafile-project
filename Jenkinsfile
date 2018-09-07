pipeline {
  agent any
   stages {
     stage ('build') {
       steps{
       sh 'mvn package'
       }
       }
       }
  post {
    always {
      archiveArtifacts artifacts:'dist/*.jar', fingerprint: true
    }
  }
  
}
       
