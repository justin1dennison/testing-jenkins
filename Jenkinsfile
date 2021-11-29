pipeline{
    agent  any
    stages{
                
        stage("Deployment"){
            when {
                changeRequest()
            }
            steps{
                echo "$env"

            }
            post{
                always{
                    echo "========Completed A: Always========"
                }
            }
        }
    }
}