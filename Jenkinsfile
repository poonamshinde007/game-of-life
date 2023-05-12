pipeline{
    agent{
	      
		  label{
		    label "built-in"
			customWorkspcae "/mnt/project2"
			   }
		}
		stages{
		 stage ("deploy"){
		   steps {
            
		     sh "mvn clean install"
		     sh "cp -r /mnt/project2/gameoflife-web/target/gameoflife.war /mnt/server/apache-tomcat-9.0.75/webapps"

		        }
		      }
		   }
		
        }
