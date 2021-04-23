pipeline{
	agent any
	tools {nodejs "MyNode"}
	stages{

		stage("Check Node version"){
			steps{
				sh "node --verison"
			}
		}

		stage("install dependencies"){
			steps{
				sh "npm --version"
				sh "npm install"
			}
		}
		stage("Test"){
			steps{
				sh "node app.js"
			}
		}
		stage("Release the version"){
			steps{
				echo "Release the version"
			}
		}

	}
}
