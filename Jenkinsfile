node{
    stage('SCM Checkout'){
    git 'https://github.com/JohannesSchwegler/mavenTest'
    }   
    stage('Compile-Package'){
        steps{
        withMaven(maven:'Maven_3_6_2'){
            sh 'mvn clean compile'   
        } 
 
    }
    }
    
    stage('Testing Stage'){
        steps{
        withMaven(maven:'Maven_3_6_2'){
            sh 'mvn test'   
        } 
 
    }
    }
    
}
