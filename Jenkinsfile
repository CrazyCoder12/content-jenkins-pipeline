pipeline {
  agent any

  stages {

    stage ('Build') {
      steps {
        sh 'javac -d'
        sh 'echo Main-Class: Rectangulator > MANIFEST.MF'
        sh 'jar -cvmf MANIFEST.MF rectangle.jar *.class'
      }
    }
  }
}
