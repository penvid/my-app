node{
  stage('SCM Checkout'){
  
      git 'https://github.com/penvid/my-app'
  }
  stage('Compile-pacakge'){
    def mvnHome = tool name: 'maven', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }

}
