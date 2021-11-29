pipeline{
    stages{
        stage("A"){
            steps{
                echo "========executing A========"
                sh 'printenv'
		echo "Working"
            }
            post{
                always{
                    echo "========Completed A: Always========"
                }
                success{
                    echo "========A executed successfully========"
                }
                failure{
                    echo "========A execution failed========"
                }
            }
        }
    }
}
