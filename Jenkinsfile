
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
    stage ('deploy to container') {
	 sh 'cp /var/lib/jenkins/workspace/jenkins/target/*.war /opt/tomcat/webapps/'
	 sh 'chmod 777 /opt/tomcat/webapps/*.war'
    }
}
