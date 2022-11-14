pipeline {
	agent{
		node{
			label "Nodojava"
		}
	}

	stages{
		stage("build"){
			steps{
				sh "mvn clean package -DskipTest"
			}
		}
	}
}

