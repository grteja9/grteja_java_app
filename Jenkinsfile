@Library('my-shared-library') _
customWorkspace='/opt/Workspace/grteja_java_app/'
pipeline{
    dir('customWorkspace')
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

    }
}