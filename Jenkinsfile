node{
	
      checkoutSCM()

      stage('Build') {
              sh  '''
	          cd todo_demo/
                  sudo flutter build apk
                  '''
            }
}

def checkoutSCM(){
    stage("Checkout SCM") {
        sh '''
		rm -rf todo_demo/
		pwd
		git clone -b master https://github.com/melwinlobo18/todo_demo.git
	   '''
    }
}
