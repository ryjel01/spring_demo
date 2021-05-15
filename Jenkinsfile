pipeline {
	agent any
	tools {
    	maven 'local-mvn'
	}
	stages {
    	stage("Checkout") {   
        	steps {               	 
            	git branch:'main', url: 'https://github.com/ryjel01/spring_demo'          	 
           	 
        	}    
    	}
    	stage('Build') {
        	steps {
        	sh "mvn compile"  	 
        	}
    	}
   	 
    	stage("Unit test") {          	 
        	steps {  	 
            	sh "mvn test"          	 
       	}
}
}
}
