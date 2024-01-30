## Level 8

 **The objective of this level is to connect as level8 without entering the password by finding the SSH key pair (private and public keys). Follow these steps:**

 - Use this command to check the public key fingerprint: 

> ssh-keygen -l -E md5 -f /home/level/08_sshz/backups/authorized_keys.backup

Despite MD5 being considered insecure, it serves our purpose here.

 - Visit the site ([https://hdm.io/tools/debian-openssl/](https://hdm.io/tools/debian-openssl/)) to download 2048-bit SSH keys.
 
 - Identify the private key corresponding to the previously identified public key.
 - Open PowerShell as an administrator. Use the `scp` command to copy the private key to the server:
 

> scp -o StrictHostKeyChecking=no -P 19198 path\to\private\key level8@warchall.net:path\to\destination

Example:
`scp -o StrictHostKeyChecking=no -P 19198 path\to\private\key level8@warchall.net:path\to\destination` 

 - Enter your password
 - Return to PuTTY and modify file permissions for owner-only read and write access with: 
 

> chmod 600 ~/private_rsa_key

 - Use the following command to connect as level8 without entering a password:

> ssh -i ~/private_rsa_key level8@warchall.net -p 19198



By following these steps, you should successfully access to the solution.

