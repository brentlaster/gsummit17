#!groovy
// starting Jenkins file for Lab 2

// * 1. Add Library annotation here

node ('worker_node1') {
   stage('Pull Source') {          
        // Get code from our git repository    
         checkout scm
   }
  
   stage('Compile') {

// * 2. modify step below to use shared-library gbuild3 routine

      sh "${tool 'gradle32'}/bin/gradle clean compileJava -x test"
   }
   
}
