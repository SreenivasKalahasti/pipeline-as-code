stage('Environment Analysis') {
         parallel {
                stage('Print All Global Variables'){
                        steps{ 
                                cmd """
                                 get-childitem env:* 
                                """
                             }
                   }
                stage('Execute Shell'){
                        steps{ 
                                cmd """
                                echo "Pipeline Test"
                                """
                             }
                   }
                stage('Display Date'){
                        steps{ 
                                cmd """
                                "Date and time is: $((Get-Date).ToString())"
                                """
                             }
                   }
                }
}
