pipeline {
  agent any
   stages {
     stage ('build') {
       steps{
       sh 'mvn clean package'
       }
       }
       }
  post {
    always {
      archiveArtifacts artifacts:'dist/*.jar', fingerprint: true
    }
  }
  
}
       
