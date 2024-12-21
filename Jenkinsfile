pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        bat 'dir'
                        bat 'copy C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\webappCD\\helm\\* .'
			bat 'dir'
                        bat 'helm upgrade --install age-calci age-calci  --set image.repository=registry.hub.docker.com/amoljorewar/age-calculator --set image.tag=latest'
              			
            }           
        }
    }
}
