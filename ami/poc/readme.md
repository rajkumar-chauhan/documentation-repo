# POC 

|CREATED/UPDATED |VERSION|AUTHOR|COMMENT|
|--------|-----------|-------|---------|
|21-06-2024|0.1|Rajkumar|Initial Commit|

## Purpose 
The Purpose of this documentation is to setup an  AMI  

## Pre-requisite
You must have a valid AWS account to setup an AMI 

## Set-up

* First of all, Go to AWS management console and login with root or IAM user. Then select EC2 by searching it on global search box.
 ![image](https://github.com/rajkumar-chauhan/documentation-repo/assets/160397769/e3f5a609-1fad-4d34-a886-0366167b61a9)

  

* Launch an instance by clicking on the right side **launch instance**
   ![Screenshot (861)](https://github.com/rajkumar-chauhan/documentation-repo/assets/160397769/08c081db-3966-4711-a9af-466d7b12d1ce)


* Configure the instance according to your need.
   ![Screenshot (862)](https://github.com/rajkumar-chauhan/documentation-repo/assets/160397769/690a2c71-16ce-4567-a2f8-2955b6bbf885)

* Then launch the instance

* Navigate to the EC2 you will find Your instance in the running state
  ![Screenshot (863)](https://github.com/rajkumar-chauhan/documentation-repo/assets/160397769/66acae2e-4def-4337-9b90-30ee38336ced)

* Once in Running state click on **action** on the upper right side of the EC2 console
* Many option will come out

* Click on **Image and template**
* Then a option will come out **create image** click on it 
![Screenshot (869)](https://github.com/rajkumar-chauhan/documentation-repo/assets/160397769/a105b8f4-0840-4c07-8b92-30b4d9e5d701)

* Your AMI is created
  ![Screenshot (872)](https://github.com/rajkumar-chauhan/documentation-repo/assets/160397769/bf41318a-aca3-4842-bf4e-0472fc9c5527)

* You can check the AMI by navigating to AMI section

* You will find your AMI there having same configuration as the initial instance with the help of which you can launch as many instance as needed by clicking on **launch instance From AMI** . The launched instance will have the same configuration as same as the initial one.
    ![Screenshot (873)](https://github.com/rajkumar-chauhan/documentation-repo/assets/160397769/2abc7bc8-28f5-4ce6-b4d7-62a979d205a0)

 
 ## Conclusion 
 By following the above prescribed steps you will able to launch AMI of the instance. 

 ## Contact information
 ## Contact Information 
|Name|Email Address|
|:---:|:---:|
|Rajkumar|rajkumar.chauhan.snaatak@mygurukulam.co|

## References
|Links|
|-----|
|https://dev.to/tanmaygi/launch-an-ec2-instance-with-ami-in-1-minute-step-by-step-guide-5g6l|
