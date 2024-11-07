pipeline{
agent any

tools {
  maven 'mymvn'
}

stages {

    stage('build') {
        steps {
            sh 'mvn clean package -DskipTests=true'
            }
     }
   stage('test') {
   parallel {
     stage('test A'){
       steps{
         echo 'echo hello world'
       }
     }
       stage('test B'){
       steps{
         echo 'echo hello world B'
       }
     }
   }
  }


}

}
