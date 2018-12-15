pipeline {
   agent any
   stages {
     stage ('compile satge') {
	   steps {
	     withMaven {maven: 'apache-maven-3.5.4'} {
		 sh 'mvn clean compile'
		}
		
	   }
	   
	 }
	   stage ('metrics satge') {
	   steps {
	     withMaven {maven: 'apache-maven-3.5.4'} {
		 sh 'mvn -p metrics pmd:pmd'
		}
		
	   }
	   
	 }
	 
   }
   
}

