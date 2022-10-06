Pipeline {
  agent {
    node {
      label 'JenkinsBuildNode'
}
}
 stages {
  stage('Code Checkout') {
    steps {
     checkout([
        $class: 'GitSCM',
        branches: [[name: 'develop']],
        userRemoteConfigs: [[credentialsId: 'Apreddys119@',url: 'https://github.com/pradeeparumalla/GitCheckout.git']]])
    }
  }
  stage('shell command') {
    steps {
   sh "ls -al" 
  }
  }
  }
}
