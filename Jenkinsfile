pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        bat 'dir'
		    	bat 'mkdir age-calci'
                        bat 'copy helm\\age-calci\\*  age-calci\\'
		        bat 'dir'
                        bat 'C:\\"Program Files"\\helm-v3.16.4-windows-amd64\\windows-amd64\\helm upgrade --install age-calci age-calci  --set image.repository=registry.hub.docker.com/amoljorewar/age-calculator --set image.tag=latest'
              			
            }           
        }
    }
}
