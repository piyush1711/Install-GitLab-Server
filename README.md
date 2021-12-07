
## kubernates_tutorials


# How To Install GitLab Server (Community Edition)

Step 1 : Update & Install CA Certificates

         sudo apt update
         
         sudo apt install ca-certificates curl openssh-server postfix
         
 Step 2: Curl a Script 
 
 
          curl -LO https://packages.gitlab.com/install/repositories/gitlab/gitlab-ce/script.deb.sh
          bash script.deb.sh
          
          
 Step 3:  Install Gitlab Community Edition 
 
          sudo apt install gitlab-ce
          
 Step 4 : Disable Fire Wall
          sudo ufw disable
          
 Step 5 : Change the External Hostname and Post 
 
            sudo nano /etc/gitlab/gitlab.rb
  In This Change 
        
           external_url 'https://example.com:PORT_NUMBER'
           
           
           
 Step 6 : Reconfigure Gitlab
 
          `sudo gitlab-ctl reconfigure`

 
