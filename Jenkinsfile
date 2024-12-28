pipelines {
  agent any 

  stages {
    stage ('Building'){
      steps {
        echo "Starting nodejs build"
        
      }
    }

    stage ("Testing'){
           steps {
            echo "Testing the build"
           }
    }

           stage ("Final cleanup"){
             steps {echo "Cleaning build"}
           }
  }
  

}
