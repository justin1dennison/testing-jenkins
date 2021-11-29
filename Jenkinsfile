pipeline{
    agent  any
    stages{
                
        stage("A"){
            steps{
                def vars = checkout(scm)
                echo "========executing A========"
                sh 'printenv'
                echo '${pullRequest}'
                echo '${vars}'
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