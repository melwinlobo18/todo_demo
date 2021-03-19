@Library('jenkins-shared-libs') _

node("srvr-app-01.lab-us.ariba.com"){
	
      checkoutSCM()

      stage('Build') {
              sh  '''
                  flutter build apk
                  '''
            }
}

def checkoutSCM(){
    stage("Checkout SCM") {
	      cleanWs()
        sh "git clone -b master git@github.com:melwinlobo18/todo_demo.git"
    }
}
