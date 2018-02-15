pipeline{
	agent any
	stage('Compile Stage'){
		withMaven(maven:'maven3.5.2'){
            sh 'mvn clean compile'
        }
    }
    stage('Build, Test and Package'){
		withMaven(maven:'maven3.5.2'){
            sh 'mvn test'
        }
    }
    stage('Deployment Stage'){
		withMaven(maven:'maven3.5.2'){
            sh 'mvn deploy'
        }
    }
}
 
