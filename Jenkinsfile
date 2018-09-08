pipeline {
  agent any
   stages {
     stage ('build') {
       steps{
       sh 'mvn -f build.xml -v'
       }
       }
       }
  post {
    always {
      archiveArtifacts artifacts:'dist/*.jar', fingerprint: true
    }
  }
  
}
       
