@Library('my-shared-library') _
customwokspace='/opt/Workspace/grteja_java_app/pom.xml'
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
                dir('customworkspace'){
                script{
                    mvnTest()
        }

 
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