
node {
    stage ('checkout scm') {
	 git 'https://github.com/srikanth1798/JavaWebCalculator.git'
	} 
	stage ('build steps') {
	 sh 'mvn validate'
	 sh 'mvn compile'
	 sh 'mvn test'
	 sh 'mvn package'
	}
}
