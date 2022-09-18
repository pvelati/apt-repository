# apt-repository

Package repository for Debian-based systems

## Compatibility

* Debian 11 (bullseye) and derivatives (Proxmox and others)

## Installation

1. **Add the repository's GPG key:**  

   ```bash
   curl -1sLf 'https://raw.githubusercontent.com/pvelati/apt-repository/master/debian/conf/key.gpg.key' | gpg --dearmor -o /usr/share/keyrings/pvelati.gpg
   ```

2. **Set up the repository:**  

   ```bash
   echo "deb [signed-by=/usr/share/keyrings/pvelati.gpg] https://pvelati.github.io/apt-repository/debian/ bullseye main" > /etc/apt/sources.list.d/pvelati.list
   ```
