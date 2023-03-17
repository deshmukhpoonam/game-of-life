pipeline {

          agent {
		  
		      label {
			  
			      label "slave-1"
				  customWorkspace "/mnt/project/"
			  }
		  }
		  
		  stages {
		  
		     stage ("package") {
			 
			     steps {
				 
				 sh "sudo rm -rf /root/.m2/repository"
				 sh "sudo mvn clean install"
				 sh "sudo cp -r /mnt/project/gameoflife-web/target/gameoflife.war /mnt/server/apache-tomcat-9.0.73/webapps"
				 
			
				 }
			 
			 
			 }
		  
