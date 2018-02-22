pipeline{
   agent any
   tools{
   maven 'Maven'
   jdk 'java-home'
   }
   stages {
     stage ('Initialize') {
        steps{
            sh '''
                echo "PATH = ${PATH}"
                echo "M2_HOME = ${M2_HOME}"
               '''
            }
   }
   stage('Build'){
        steps{
            sh 'mvn install'
         }
      }
   }
}
