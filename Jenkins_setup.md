## Install Jenkins in Ubuntu 18.04

 Step 1) Check the Upadates
        
        `sudo apt update`
   
 Step 2) Check Java Version As Java as Necessery
 
      java -version
    
 Step 3) If not present Install Java
 
      `sudo apt install default-jre`
      `java -version`
       
 Step 4) Now add Key and 
 
      `wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -`
      `sudo sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'`
      
 Step 5) Install Jenkins
      
      `sudo apt update`
      `sudo apt install jenkins`
      
 Step 6) Now start Jenkins & Check Status of Jenkins
 
      `sudo systemctl start jenkins`
      `sudo systemctl status jenkins`
      
 Step 7) Allow Firewall  
 
      `sudo ufw allow 8080`
      
 Step 8) Check Password 
 
     `cat /var/lib/jenkins/secrets/initialAdminPassword`
  
