pipeline {
	agent any
	stages {
		stage('build') {
			steps {
<<<<<<< HEAD
				sh 'javac -d. src/*.java'
				sh 'echo Main-Class: Rectangulator > MANIFEST.MF'
				sh 'jar -cvmf MANIFEST.MF rectangle.jar *.class'
=======
				sh 'javac . src/.java'
				sh 'echo Main-Class: Rectangulator > MANIFEST.MF'
				sh 'jar -cvmf MANIFEST.MF rectangle.jar .class'
>>>>>>> 124e95b52a94880a074714d5764e5dd91b9223e5
			}
		}
		stage('run') {
			steps {
				sh 'java -jar rectangle.jar 7 9'
			}
		}
	}
	post {
		success {
			archiveArtifacts artifacts: 'rectangle.jar', fingerprint: true
		}
	}
}
