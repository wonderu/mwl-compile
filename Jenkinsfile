timestamps {

node ('docker') { 

	stage ('Dockers/OSCross Compile - Checkout') {
 	 checkout scm
	}
	stage ('Dockers/OSCross Compile - Build') {
sh """ 
docker build --pull --rm -f "Dockerfile" -t mwlcompile:latest "." 
 """ 
	}
}
}