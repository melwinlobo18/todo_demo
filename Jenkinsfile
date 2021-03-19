node{
	
      checkoutSCM()

      stage('Build') {
              sh  '''
	      	  sudo su
	      	  export PATH=$PATH:/home/melwinlobo18/snap/flutter/common/flutter/bin
		  echo $PATH
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
