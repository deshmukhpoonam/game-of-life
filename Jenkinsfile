/* pipeline {
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
*/

pipeline{
 agent {
  label {

     label "built-in"
     customWorkspace "/mnt/newdata"
        }
    }

 stages {
 stage ("deploy-on-tomact"){
 steps {
        sh "mvn clean install"
        sh "docker run -itdp 99:8080 --name new1 tomcat"
        sh "cp /mnt/newdata/gameoflife-web/target/webapps/gameoflife.war /mnt/newdata/usr/local/tomcat"

       }
  }

 }

}
