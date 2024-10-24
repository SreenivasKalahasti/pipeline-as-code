stage('Environment Analysis') {
         parallel {
                stage('Print All Global Variables'){
                        steps{ 
                                get-childitem env:* 
                             }
                   }
                stage('Execute Shell'){
                        steps{ 
                                echo "Pipeline Test"
                             }
                   }
                stage('Display Date'){
                        steps{ 
                                echo "Date and time is: $((Get-Date).ToString())"
                             }
                   }
                }
}
