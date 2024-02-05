# KeePass-kdbx.config
On this repos, we can bypass the root user protected password saved with .ppk using puttygen with .id_rsa and .pem. You can use the sample file above.


To convert the .ppk file using id_rsa, we can use puttygen:(install if you don't have).
Command: **1. $puttygen key.ppk -O private-openssh -o id_rsa** **2. chmod 600 id_rsa** **3. ssh -i id_rsa root@domain.com**. In that you will be directed to the machine as root user. 


To convert the .ppk file using .pem, we can use puttygen:(install if you don't have).
**1. $puttygen key.ppk -O private-openssh -o root.pem** **2. chmod 600 id_rsa** **3. ssh -i root.pem root@domain.com**

