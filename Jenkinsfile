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
                stage('Display Date'){
                        steps{
                                Script {
                                    def now=new Date()
                                    println now.format("yyMMdd.HHmm",TimeZone.getTimeZone('UTC'))
                                 }
                             }
                   }
                }
}
