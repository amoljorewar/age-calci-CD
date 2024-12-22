pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        bat 'dir'
                        //bat 'copy C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\webappCD\\helm\\*.* C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\webappCD'
			//bat 'dir'
		    	bat 'cd helm\\age-calci\\templates'
		    	bat 'dir'
                        bat 'kubectl apply -f age_calci.yaml'
		    	bat 'kubectl apply -f age_calci_svc.yaml'
		    	bat 'kubectl get all -o wide'
              			
            }           
        }
    }
}
