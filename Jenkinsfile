stage('Environment Analysis') {
         parallel {
                stage('Print All Global Variables'){
                        steps{ 
                                powershell(". get-childitem env:*") 
                             }
                   }
                stage('Execute Shell'){
                        steps{ 
                                powershell("echo Pipeline Test")
                             }
                   }
                }
}
