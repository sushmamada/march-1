pipeline {
    agent any
    stages {
        stage('git clone') {
            steps {
		git branch: 'master', url: 'https://github.com/sushmamada/march-1.git'
             }
             }
	 stage('maven version') {
           steps {	 
		 sh 'mvn --version'
	     }
	     }
	    stage('maven clean') {
             steps {	 
	         sh 'mvn clean'
	     }
	     }			
	    stage('maven validate') {
              steps {	 
		 sh 'mvn validate'
	     }
	     }		
	    stage('maven compile') {
               steps {	 
		 sh 'mvn compile'
	     }
	     }		
	    stage('maven test') {
                steps {	 
		  sh 'mvn test'
	     }
	     }		
             stage('maven package') {
                  steps {	 
		    sh 'mvn package'
	     }
	}

    }
}
