pipeline {
  agent { label "agent1" }
  stages {
    stage("build") {
       steps {
        sh """
          docker build -t hello_there .
        """
       }
    }
    stage("run") {
     steps {
      sh """
        dsocker run  --rm hello-there
      """
     }
    }
  }
}
