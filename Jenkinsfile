pipeline {
	agent any 
	stages{
		stage('1-clonecode'){
			steps{
			checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github-creds', url: 'https://github.com/etechDevops/team6-demo1.git']])
			}
		}
		stage('2-s2'){
			steps{
				sh 'lscpu'
				sh 'whoami'
			}
		}
		stage('3-s3'){
			steps{
				sh 'df -h'
				sh 'touch team6'
			}
		}
		stage('4-s4'){
			steps{
				sh 'pwd'
				sh 'du -h'
			}
		}
        stage('5-s5'){
            steps{
                echo "welcome to Jenkinsfile"
            }
        }
	}
}
