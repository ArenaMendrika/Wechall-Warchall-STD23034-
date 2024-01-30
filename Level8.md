## Level 8 (SSH... Z is sleeping)

 The objective of this level is to connect as level8 without entering the password by finding the SSH key pair (private and public keys). Follow these steps:

 - Use this command to check the public key fingerprint: 

       `ssh-keygen -l -E md5 -f /home/level/08_sshz/backups/authorized_keys.backup`

Despite MD5 being considered insecure, it serves our purpose here.

 - Visit the site ([https://hdm.io/tools/debian-openssl/](https://hdm.io/tools/debian-openssl/)) to download 2048-bit SSH keys.
 
 - Identify the private key corresponding to the previously identified public key.
 - Open PowerShell as an administrator. Use the `scp` command to copy the private key to the server:
 

       `scp -o StrictHostKeyChecking=no -P 19198 "C:\path\to\your\private\key\private_key_file" user@warchall.net:destination_folder/` 


 - Enter your password
 
 - Return to PuTTY and modify file permissions for owner-only read and write access with: 
 

   `chmod 600 ~/private_key_file`     (The tilde (~) represents my home directory, as that's where I've placed my private key. However, you can change it based on where you've placed yours.)

 - Use the following command to connect as level8 without entering a password:


   `ssh -i ~/private_key_file level8@warchall.net -p 19198`



By following these steps, you should successfully access to the solution.



