pipeline {
  agent any
  stages {

    stage('Compile') {
      steps{
        sh 'sudo /home/ubuntu/apache-maven-3.9.8/bin/mvn clean compile'
      }
    }

    stage('UnitTest') {
      steps{
        sh 'sudo /home/ubuntu/apache-maven-3.9.8/bin/mvn clean test'
      }
    }

    stage('Package') {
      steps{
        sh 'sudo /home/ubuntu/apache-maven-3.9.8/bin/mvn clean package'
      }
    }
  }
}
