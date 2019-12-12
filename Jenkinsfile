node{
  stage('SCM Checkout'){
  
      git 'https://github.com/penvid/my-app'
  }
  stage('Compile-pacakge'){
    def mvnHome = tool name: 'maven', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }

  stage('email notifiaction'){
    mail bcc: '', body: '''Hi dumbo,
    thanks''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'svidya2007@gmail.com'
    
  }  
}
