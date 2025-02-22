pipeline{
    tools{
        jdk "JAVA_HOME_LINUXSLAVE"
        maven "MAVEN_HOME_LINUXSLAVE"
    }
	agent {label 'linuxslave'}
	stages{
		stage('git clone'){
	steps{
	git 'https://github.com/BikashPanda1998/maven_test.git'
		}
	}
	stage('compile'){
	steps{
	sh 'mvn compile'
    echo 'compile completed successfully'	
    	}
	}
	stage('test'){
	steps{
        sh 'mvn test'
	echo 'test completed successfully'
		}
	}
	stage('package'){
	steps{
        sh 'mvn package'
	echo 'package completed successfully'
		}
	}
	}
}
