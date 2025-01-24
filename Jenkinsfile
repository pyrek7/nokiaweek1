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
            }
        }
        stage('Scripting') {
            steps {
                parallel(
                    "TaskOne":{
                        echo 'task one job1'
                        echo 'task one job2'
                    },
                    "TaskTwo":{
                        echo 'task two job1'
                        echo 'task two job2'
                    }
                )
            }
        }
    }
}
