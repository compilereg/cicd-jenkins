pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
		VAL=$(./add 1 2)
		if [ ${VAL} -ne 3 ]
		then
			echo "Failed testing.."
			exit 1
		else
			echo "OK Testing..."
		fi
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
