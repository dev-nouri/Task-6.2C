pipeline{
    agent any
    environment{
        DIRECTORY_PATH="path/directory/code"
        TESTING_ENVIRONMENT="testing-environment"
        PRODUCTION_ENVIRONMENT="SIT223"
    }

    stages
    {
        stage("Build"){
            steps{
                echo "fetched the code from $DIRECTORY_PATH"
                echo "Building completed..."
            }
        }

        stage("Unit and Integration Test"){
            steps{
                echo "Unit test"
                echo "Integrated test"
                echo "Testing completed..."
                mail to: "mnouri.2002.10@gmail.com",
                subject: "Unit and Integration Test",
                body: "Testing completed"
            }
        } 
        stage("Code Analysis"){
            steps{
                echo "Testing the code and analysing"
                echo "Analysing completed..."
            }
        }
        stage("Security Scan"){
            steps{
                echo "Scanning for vulnerability"
                echo "Scanning completed..."
                mail to: "mnouri.2002.10@gmail.com",
                subject: "Security Scan",
                body: "Security Scan completed"
            }
        }
        stage("Integration test on Staging"){
            steps{
                echo "Testing to see if it functions as expected"
                echo "Completed..."
            }
        }
        stage("Deploy to Prodcution"){
            steps{
                echo "Deployed to production completed"
            }
        }
    }
}
