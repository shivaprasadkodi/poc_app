node {
      stage('SCM Checkout'){      
      git 'https://github.com/nagbabuk/poc_app'
      }
      stage('Compile-Package'){
            //getting ant path         
           def antHome = tool name: 'ant', type: 'ant'
           env.JAVA_HOME = tool name: 'java', type: 'jdk'
           sh "${antHome}/bin/ant war"
      }
      stage('Deploy-tomcat'){
            
            
            steps {
                //sh 'echo "Hello World"'
                sh 'scp /var/lib/jenkins/workspace/test/dist/lib/*.war /opt/tomcat/webapps/'
            }
       //sshagent(['test-ubuntu']) {
    // some block
             
       //}     
      }


}
