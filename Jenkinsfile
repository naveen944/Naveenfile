node{
	stage('SCM checkout'){
		git 'https://github.com/javahometech/my-app'
	}
	
	stage('compile-package'){
		def mvnHome=tool name: 'Maven 3.6.1', type: 'maven'
		sh "${mvnHome}/bin/mvn package"
	}
}
