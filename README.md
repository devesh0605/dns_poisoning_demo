# DNS poisoning demonstration
DNS cache poisoning, also known as DNS spoofing, is a type of attack that exploits vulnerabilities in the domain name system (DNS) to divert Internet traffic away from legitimate servers and towards fake ones. One of the reasons DNS poisoning is so dangerous is because it can spread from DNS server to DNS server.

# Requirements
VMware Workstation, ubuntu 12.04 VMware image, PC with the requirements of VMware, a stable internet connection and a basic knowledge of network commands.

# The steps are as follows:-

## Step 1: Scouting the target
<img width="50%" src="https://github.com/devesh0605/dns_poisoning_demo/blob/master/Step%201.png" alt="Image 1">

Visit the website which you wanna access with a different URL.

## Step 2: Gaining info on your target
<img width="50%" src="https://github.com/devesh0605/dns_poisoning_demo/blob/master/Step%202.png" alt="Image 2">

Use the `nslookup` command to find about the IP addresses of the target website and the website you want to replace it with.
Nslookup (stands for “Name Server Lookup”) is a useful command for getting information from DNS server. It is a network administration tool for querying the Domain Name System (DNS) to obtain domain name or IP address mapping or any other specific DNS record. It is also used to troubleshoot DNS related problems.

## Step 3: Accessing file that contains IP addresses
<img width="50%" src="https://github.com/devesh0605/dns_poisoning_demo/blob/master/Step%203.png" alt="Image 3">

Run the command `sudo nano /etc/hosts`.
`sudo` is used to access the files as the system administration.
`nano` is used to open the code editor to edit `/etc/hosts`.Use your admin password.

## Step 4: The file opens
<img width="50%" src="https://github.com/devesh0605/dns_poisoning_demo/blob/master/Step%204.png" alt="Image 4">

The upper window should open.

## Step 5: Editing the file
<img width="50%" src="https://github.com/devesh0605/dns_poisoning_demo/blob/master/Step%205.png" alt="Image 5">

Make the DNS entry in the file. The syntax should be `IP_address_of_arget_website URL_of_website_you_want_to_replace_it`
Save the file.

## Step 6: Checking the result.
<img width="50%" src="https://github.com/devesh0605/dns_poisoning_demo/blob/master/Step%206.png" alt="Image 6">

Visit the `URL_of_website_you_want_to_replace_it` and your target website will open AND that's how it's done....

Enjoy and Thank you!!!!
