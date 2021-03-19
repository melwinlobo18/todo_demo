node{
	
      checkoutSCM()

      stage('Build') {
              sh  '''
                  flutter build apk
                  '''
            }
}

def checkoutSCM(){
    stage("Checkout SCM") {
        sh "git clone -b master git@github.com:melwinlobo18/todo_demo.git"
    }
}
