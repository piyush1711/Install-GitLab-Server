# If DPKG Error like below 

            E: Could not get lock /var/lib/dpkg/lock - open (11 Resource temporarily unavailable)
            E: Unable to lock the administration directory (/var/lib/dpkg/) is another process using it? 
            
            
            
## Solution of it is 
     sudo rm /var/cache/apt/archives/lock
     sudo rm /var/lib/dpkg/lock
     sudo rm /var/lib/apt/lists/lock
