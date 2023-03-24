pipeline {
 agent {
  label {
  
     label "built-in"
	 customWorkspace "/mnt/container"
        }
     
	    }

  stages {
   
      stage ("deploy-on-doc-httpd"){
	   steps {
	      sh "docker run -itdp 90:80 --name httpdnew httpd bash"
	      sh "mvn clean install"
	      sh "cp -r  /mnt/container/gameoflife-web/target/gameoflife.war httpdnew:/usr/local/apache2/htdocs"
		 
	   
	   }
	  
	 }
  
  }
}
