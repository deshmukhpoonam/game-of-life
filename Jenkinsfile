pipeline{
    agent{
	    label {
		    label "built-in"
			customWorkspace "/mnt/project"
			   }
		}
		stages {
		 stage ("deploy"){
		    steps {
		     sh "mvn clean install"
		     sh "cp -r /mnt/project/gameoflife-web/target/gameoflife.war /mnt/server/apache-tomcat-9.0.73"
		      sh "chmod -R 777 /mnt"

		        }
		      }
		   }
		
        }
