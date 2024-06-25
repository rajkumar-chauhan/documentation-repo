#  POC on Dynamic Application Security Testing (DAST) for Java Application

|CREATED/UPDATED |VERSION|AUTHOR|COMMENT|
|--------|-----------|-------|---------|
|25-06-2024|0.1|Rajkumar|Initial Commit|

## Table of Content: 
- [Introduction](#Introduction)
- [Pre-requisites](#Pre-requisites)
- [Step-by-Step setup Guide](#Step-by-step-Setup-Guide)
- [Conclusion](#Conclusion)
- [Contact Information](#Contact-Information)
- [References](#References)
  
## Introduction
This Proof of Concept (POC) aims to demonstrate the effectiveness of DAST in identifying security vulnerabilities in Java applications. 
Dynamic Application Security Testing (DAST) involves evaluating a live application for security vulnerabilities by emulating external threats. OWASP ZAP (Zed Attack Proxy) is a widely used open-source DAST tool designed to detect security flaws in web applications.

## Pre-requisites
- [OWASP ZAP](#https://www.zaproxy.org/) 
- A Running Application(JAVA) to Perform DAST.  
  ![Screenshot 2024-06-25 114014](https://github.com/rajkumar-chauhan/documentation-repo/assets/160397769/ad560f7f-73e1-4820-8e00-e600da9dad06)

---

## Step-by-Step Setup Guide

**Step 1**: Update Your Linux System

Before installing OWASP ZAP, it's essential to update your system to ensure that you have the latest packages and security patches. To update your system, open the terminal and type the following command:
```
sudo apt update
```
![Screenshot 2024-06-24 061433](https://github.com/rajkumar-chauhan/documentation-repo/assets/160397769/44ee1b16-155f-435e-ab90-eb790b0c80c8)

---

**Step 2**: Install OWASP ZAP

Once your system is up to date, you can install OWASP ZAP. To do so, type the following command in the terminal:
```
sudo snap install zaproxy --classic
````
![Screenshot 2024-06-24 062911](https://github.com/rajkumar-chauhan/documentation-repo/assets/160397769/37f7cd30-11a9-4c24-936b-3e73c7fda3b0)

----

**Step 3**: Launch OWASP ZAP

Once the installation is complete, you can launch OWASP ZAP from the application menu or the command line. To launch it from the command line, type the following command:
```
zaproxy
```
![Screenshot 2024-06-24 063424](https://github.com/rajkumar-chauhan/documentation-repo/assets/160397769/8ff6e5cc-e4f7-46f4-8f6e-22c62a450fab)

You can now start using OWASP ZAP to test the security of your web applications.After a few minutes, OWASP ZAP will open up.
![Screenshot 2024-06-24 064348](https://github.com/rajkumar-chauhan/documentation-repo/assets/160397769/2528e337-8781-4b76-945f-9af79eab4932)

----

**Step 4**: Click on the **Automated scan** option a interface will come out on which provide the URL of the application and click on **attack**. 
![Screenshot 2024-06-25 113128](https://github.com/rajkumar-chauhan/documentation-repo/assets/160397769/2575a0c0-d65a-421b-bc8a-13b0c253c99d)

OWASP ZAP will start  scanning  your application for  vulnerabilities .

![Screenshot 2024-06-25 113913](https://github.com/rajkumar-chauhan/documentation-repo/assets/160397769/4ebd19a2-4d8e-4419-9054-6aad549fe4d6)

----

 **Step 5** : Analyze Results

 After the scan, navigate to the Alerts tab to see the list of identified vulnerabilities. Click on each **alert** to see details .
 ![Screenshot 2024-06-25 112229](https://github.com/rajkumar-chauhan/documentation-repo/assets/160397769/8ea76600-e339-4cf5-93f3-0c13d36bbcd0)

 ![Screenshot 2024-06-25 113550](https://github.com/rajkumar-chauhan/documentation-repo/assets/160397769/4fda7824-0a7f-43ef-99a2-191824fc247f)



----

**Step 6** : Report Generation: 

You can also Generate the Report of the analysis by click on the **Report** option and generate it in desired format (HTML, PDF,JSON etc.) for future References. 
![Screenshot 2024-06-25 115413](https://github.com/rajkumar-chauhan/documentation-repo/assets/160397769/6bdfc77f-d8b1-4290-99c5-20bee91a71d1)

After selecting the format,click on **Generate Report**. Your Report will be generated in your desired directory. 
![Screenshot 2024-06-25 115337](https://github.com/rajkumar-chauhan/documentation-repo/assets/160397769/44d911d7-018e-483c-a2dc-364fa858de82)

## Conclusion

Dynamic Application Security Testing (DAST) is a crucial method for identifying security vulnerabilities in live applications by simulating real-world attacks. OWASP ZAP, as a leading open-source DAST tool, plays a vital role in uncovering and addressing security issues in web applications, thereby enhancing their resilience against potential threats. By integrating DAST tools like OWASP ZAP into the security testing process, organizations can proactively protect their applications and ensure a robust security posture.


## Contact Information 

|Name|Email Address|
|:---:|:---:|
|Rajkumar|rajkumar.chauhan.snaatak@mygurukulam.co|

## References 
| Links |
|--------|
|https://techofide.com/blogs/how-to-install-owasp-zap-on-windows-and-linux/|
|https://www.zaproxy.org/|





