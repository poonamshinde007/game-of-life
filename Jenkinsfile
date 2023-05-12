pipeline{
    agent{
	      
		  label{
		    label "built-in"
			customWorkspace "/mnt/project3"
			   }
		}
		stages{
		 stage ("deploy"){
		   steps {
            
		     sh "mvn clean install"
		     sh "cp -r /mnt/project3/gameoflife-web/target/gameoflife.war /mnt/server/apache-tomcat-9.0.75/webapps"

		        }
		      }
		   }
		
        }
