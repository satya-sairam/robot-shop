pipeline{
   agent any
   stages{
     stage('git checkout'){
        steps{
            sh '''
              git clone https://github.com/satya-sairam/robot-shop.git
              cd shipping
              mvn clean package
            '''

        }
     }
      stage('checking'){
             steps{
                 sh '''
                   cd shipping
                   mv target/*.jar  shipping.jar
                 '''

             }
          }


   }



}