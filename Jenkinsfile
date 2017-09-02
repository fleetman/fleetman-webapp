node {
   stage('Preparation') { 
      git 'https://github.com/fleetman/fleetman-webapp'
   }
   stage('Build') {
      sh "mvn package"
   }
   stage('Results') {
      //junit '**/target/surefire-reports/TEST-*.xml'
      archive 'target/*.jar'
   }
}
