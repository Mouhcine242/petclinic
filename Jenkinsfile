pipeline {
	agent any
    stages {
        stage('Build on k8s ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install petclinic-app petclinic  --set image.repository=crdemo6.azurecr.io/06062000/petclinic '
              			
            }           
        }
    }
}
