node {
   stage('Source') {
       git 'https://github.com/johnhaire/time-tracker.git'
   }
   stage('Build') {
       def mvnHome = tool name: 'Maven 3', type: 'maven'
       bat "${mvnHome}/bin/mvn clean package"
   }
}
