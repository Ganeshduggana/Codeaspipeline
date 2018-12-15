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
	   stage ('Testing Stage') {
	   steps {
	     withMaven {maven: 'apache-maven-3.5.4'} {
		 sh 'mvn test'
		}
		
	   }
	   
	 }
	 stage ('Package Stage') {
	   steps {
	     withMaven {maven: 'apache-maven-3.5.4'} {
		 sh 'mvn package'
		}
		
	   }
	   
	 }

   }
   
}

