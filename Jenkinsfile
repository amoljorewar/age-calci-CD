pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        bat 'dir'
		    	bat 'mkdir age-calci'
		    	bat 'mkdir age-calci\\templates'
                        bat 'copy helm\\age-calci\\*  age-calci\\'
		    	bat 'copy helm\\age-calci\\templates\\* age-calci\\templates\\'
		        bat 'dir'
                        bat 'helm upgrade --install age-calci age-calci  --set image.repository=registry.hub.docker.com/amoljorewar/age-calculator --set image.tag=latest'
              		
            }           
        }
    }
}
