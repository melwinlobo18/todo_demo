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
        sh '''
		rm -rf todo_demo/
		git clone -b master https://github.com/melwinlobo18/todo_demo.git
	   '''
    }
}
