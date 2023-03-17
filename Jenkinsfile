pipeline {

          agent {
		  
		      label {
			  
			      label "built-in"
				  customWorkspace "/mnt/project/"
			  }
		  }
		  
		  stages {
		  
		     stage ("package") {
			 
			     steps {
				 
				 sh "rm -rf /root/.m2/repository"
				 sh "mvn clean install"
				 sh "cp -r /mnt/project/gameoflife-web/target/gameoflife.war /mnt/server/apache-tomcat-9.0.73/webapps"
				 
			
				 }
			 
			 
			 }
		  
		  
		  
		 		  }

