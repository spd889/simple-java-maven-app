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
        steps {
            echo "hello world"
            }
     }

}

}
