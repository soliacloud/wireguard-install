# Wireguard vpn-server - Automated installing script

# Prepare your Linux Server:
__Make sure you have a Linux server (Ubuntu or Debian is always recommended) and administrative access to it. You can also use a virtual private server (VPS) from [Solia.Cloud](https://solia.cloud/)__

# SSH into Your Server:
*Log in to your server via SSH:*

``
ssh your_username@your_server_ip ``

# Update Your System:

*First, update your system's package list and upgrade the installed packages:*

``sudo apt update && upgrade``

# Install Git:

*If Git is not already installed on your server, you can install it:*

``sudo apt install git``

# Download and Run Wireguard Installer:

There is already a official easy & secure installation script for Wireguard. To download and run it, use the following commands:

``git clone https://github.com/Nyr/wireguard-install``

``cd wireguard-install``

``sudo bash wireguard-install.sh``

_Note: The installer will ask you some configuration questions. You can typically accept the default values, but make sure to specify a custom DNS if needed._

# Configuration:

Follow the on-screen instructions to configure WireGuard based on your preferences.

# User Management:

After the installation is complete, the script will provide you with a link to download your WireGuard client configuration files. Download these files to your local machine.

# Start the WireGuard Service:

``sudo systemctl start wg-quick@wg0``

# Enable WireGuard on Boot:

``sudo systemctl enable wg-quick@wg0``

_You've now successfully set up a WireGuard server on your Linux server using a GitHub-hosted installation script. to confirm your traffic is going through the VPN._

_*Please note that the specific commands and details may vary depending on your Linux distribution. Be sure to consult the official documentation for your distribution if you encounter any issues or require more specific instructions.*_

**That's it!**
