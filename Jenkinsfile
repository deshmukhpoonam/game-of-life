pipeline{
    agent{
	    label {
		    label "built-in"
			custmWorkspcae "/mnt/project"
			   }
		}
		stages {
		 stage ("deploy"){
		    steps {
		     sh "mvn install"
		     cp -r /mnt/project/gameoflife-web/target/gameoflife.war /mnt/server/apache-tomcat-9.0.73

		        }
		      }
		   }
		
        }
