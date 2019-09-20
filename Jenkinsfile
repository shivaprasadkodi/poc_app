node {
      stage('SCM Checkout'){      
      git 'https://github.com/nagbabuk/poc_app'
      }
      stage('Compile-Package'){
      sh 'ant war'
      }
}
