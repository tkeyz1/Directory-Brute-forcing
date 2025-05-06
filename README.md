# Directory-Brute-forcing


## Objective
Discover hidden directories and sensitive files.

### Skills Learned
- Understanding the  directory structure and web server behavior

- Gained proficiency with DirBuster, Dirsearch, Gobuster, and wfuzz.
  
- Configured wordlists effectively to maximize discovery of hidden resources.

- Understand the importance of including common admin panels, backup files, config files, and other sensitive paths.

- Interpret HTTP status codes (200, 301, 403, 404, 500) to differentiate between valid and invalid directories.
  
- Identified false,positives and handle rate limiting or blocking mechanisms.

- Used techniques to evade WAFs or filters, such as URL encoding, case variations, or adding trailing slashes.

- Document discovered directories and files with potential security impact.
  
- Prioritized findings for further manual testing or exploitation.

### Tools Used

- DirBuster
- Nikto
- Gobuster
- Dirsearch
- wfuzz
- Custom wordlists (SecLists, custom-generated)

## Steps

## 1. Initial Reconnaissance
- Perform basic scanning of the target web server using nmap to identify live hosts and open HTTP/HTTPS ports.

  ![image](https://github.com/user-attachments/assets/35d61617-8050-4f00-b2c6-5f4c9ed17757)

- Confirm the web server is accessible and note the server type and version if possible.

  ![image](https://github.com/user-attachments/assets/ce0026bb-c57d-4195-9048-08f00b40b383)

### 2. Gather Information About the Target
- Collected publicly available information about common directories or files related to the target’s technology stack.

### 3. Select Wordlists
- Choosed appropriate wordlists from  customized lists based on the target’s profile.

  ![image](https://github.com/user-attachments/assets/dc654c09-a12b-4be5-899a-a37535f0807a)

- Included common directories, admin panels, backup files, config files, and other sensitive paths.

  ![image](https://github.com/user-attachments/assets/cc3ed736-f4a1-40a3-ae64-78e20033c281)


### 4. Run Directory Brute-Forcing Tool
- Useed Gobuster tool to start brute-forcing directories and files.

  ![image](https://github.com/user-attachments/assets/8e22b5cd-8909-4183-a822-46a68e330f8d)

### 5. Analyze Responses
- Monitor HTTP status codes to identify valid directories (e.g., 200 OK, 301/302 redirects).

  ![image](https://github.com/user-attachments/assets/17194e37-73e6-40d9-9d84-284ed9bca614).
  


