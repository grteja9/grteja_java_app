@Library('my-shared-library') _
pipeline{
    
        agent any
    
            stages{
                stage('Git Checkout'){
                    steps{
                        script{
                        
                            gitCheckout(
                            branch: "main",
                            url:"https://github.com/grteja9/Jenkins_Shared_Lib.git"
            )
        }
    }
}
        stage('Unit Test Maven'){
            steps{
                script{
                    mvnTest()
        }

 }
}

        stage('Integration Test Maven'){
            steps{
                script{
                    mvnIntegrationTest()
        }

 }
}

    }
}