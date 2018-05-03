pipeline {
      agent any

      stages {	
         stage('build') {
            steps {
               sh 'ant -f build.xml -v'
	    }		
         }
      }
	post { 
		always { 
	     	archiveArtificats artificates: 'dist/*.jar', fingerprint : true
            }
	}	
   }
