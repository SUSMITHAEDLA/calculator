pipeline {
  agent any
  stages {

    stage('Compile') {
      steps{
        sh '/opt/maven/bin/mvn clean compile'
      }
    }

    stage('UnitTest') {
      steps{
        sh '/opt/maven/bin/mvn clean test'
      }
    }

    stage('Package') {
      steps{
        sh '/opt/maven/bin/mvn clean package'
      }
    }
  }
}
