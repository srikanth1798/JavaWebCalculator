
node {
    stage ('checkout scm') {
	 git ''
	} 
	stage ('build steps') {
	 sh 'mvn validate'
	 sh 'mvn compile'
	 sh 'mvn test'
	 sh 'mvn package'
	}
}
