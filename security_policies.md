1.) Do security groups support both "allow" and "deny" rules? Explain how they handle traffic filtering.
No, they do not support deny rules, they contain allow rules only.
Security groups handle traffic filtering by acting as a virtual firewall which controls inbound and outbound traffic to and from EC2 instances.

2). Describe what happens to all inbound traffic by default, and explain what happens to all outbound traffic by default if left unrestricted.
By default, inbound traffic is blocked, following the cyber security principle of least privilege.
By default, all outbound traffic is allowed unless restricted. If left unrestricted, the instance can send traffic anywhere.


3.) Are EC2 instances internally aware of the security groups applied to them, or are they applied externally? Can one security group be reused across multiple instances?
The EC2 instance is not internally aware of security groups. They are applied externally and can be used across multiple instances.

 Match each port number with its precise protocol name and purpose:

Port 22 - (SSH & SFTP) Access Linux instances using terminal & Secure file transfers.
Port 21 - (FTP) Transfer files to a shared folder.
Port 80 - (HTTP) Access websites without SSL.
Port 443 - (HTTPS) Access websites with SSL encryption.
Port 3389 - (RDP) Remote access to Windows instances.
