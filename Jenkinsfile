pipeline{
    tools{
        jdk "JAVA_HOME_WINSLAVE"
        maven "MAVEN_HOME_WINSLAVE"
    }
	agent { label 'winslave'}
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
