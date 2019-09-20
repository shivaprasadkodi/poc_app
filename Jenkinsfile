node {
      stage('SCM Checkout'){      
      git 'https://github.com/nagbabuk/poc_app'
      }
      stage('Compile-Package'){
            //getting ant path
           def antHome = tool name: 'ant', type: 'ant'      
            sh "${antHome}/bin/ant war"
      }
}
