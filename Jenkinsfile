pipeline {
	agent any
    stages {
        stage('Build on k8s ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		                sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install petclinic-app petclinic  --set image.repository=acrimghub.azurecr.io/acrimghub/petclinic --set image.tag=1'
              			
            }           
        }
    }
}
