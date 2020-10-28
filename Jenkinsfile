pipeline{
	agent any
	stages{
		stage('clone'){
			steps{
				sh "rm -rf *"
				sh "git clone https://github.com/YanBarche/Jenkins.git"

			}
		}
		stage('build'){
			steps{
				sh "cd Jenkins && javac Main.java"
			}
		}
		stage('run'){
			steps{
				sh "cd Jenkins && java Main"
			}
		}
	}
}