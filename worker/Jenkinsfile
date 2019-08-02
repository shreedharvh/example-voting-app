pipeline{
    agent any
    
    tools{
	maven 'Maven 3.6.1'
    }

    stages{
        stage(build){
            steps{
                echo 'building worker app'
		dir('worker'){
                	sh 'maven compile'
		}
            }
        }
        stage(two){
            steps{
                echo 'Beautiful day to you!'
            }
        }
        stage(three){
            steps{
                echo 'Good bye!'
                sleep 5
            }
        }
    }
    post{
        always{
            echo 'Always a happy day!'
        }
    }
}
