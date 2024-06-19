# Home services
Personal Home networking and services configurations  

## Installed Services 

### VPN Pritunl
Installed on VM1  

### DNS BIND9
Docker running on VM1  
1 zone configured:  
arpa.zone (sadly cant use names .home or .local as they are not top-level-domains)  

### PLEX Media Server
Installed on Windows Server 2019  
Additionally Plex Media Server Service is installed for startup  

### NGINX
SWAG is used, with a custom configuration for IMMICH webserver.

### SAMBA
Installed on Windows Server 2019  
Used for sharing PLEX movie library to add new movies and for sharing archive folders.

## Port forwarding
18646  -> 18646  # VPN  
32400  -> 32400  # PLEX  
443    -> 443    # IMMICH
80     -> 80     # IMMICH (loopback)

