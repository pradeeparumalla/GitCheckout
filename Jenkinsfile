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
        userRemoteConfigs: [[credentialsId: '1-a-2-b-c',url: 'https://company.bitbucket.org/git.git']]])
    }
  }
  stage('shell command') {
    steps {
   sh "ls -al" 
  }
  }
  }
}
