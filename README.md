 I added the IP address of the machine to the hosts file, performed an Nmap scan to identify open ports (22 SSH and 80 HTTP), and then investigated the possibility of exploiting LFI through the page parameter. By using http://lo-fi.thm/?page=../../../../etc/passwd, I retrieved the system's user list and then found the flag at http://lo-fi.thm/?page=../../../flag.txt. This project demonstrates how LFI works and the risks it poses.
