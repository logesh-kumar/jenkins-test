piperline {
  agent { label "linux" }
  stages {
    stage("build") {
       steps {
        sh """
          dockeer build -t hello_there .
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
