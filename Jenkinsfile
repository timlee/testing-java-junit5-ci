pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'this is the build job'
        echo %JAVA_HOME% 
        echo %JRE_HOME%
        echo %MAVEN_HOME% yields
        sh 'mvn compile'
      }
    }

    stage('test') {
      steps {
        echo 'this is the test job'
        sh 'mvn clean test'
      }
    }

    stage('package') {
      steps {
        echo 'this is the package job'
        sh 'mvn package -DskipTests'
      }
    }

  }
  tools {
    maven 'mvn'
  }
  post {
    always {
      echo 'this pipeline has completed...'
    }

  }
}
