
# Long-Context Prompt

## Prompt

"I'm experimenting with using a large language model to generate a complete Ansible playbook for setting up a new web server.

The playbook should be comprehensive and include the following:
- **Base configuration:**
  - Update the package cache.
  - Install common packages (e.g., `ufw`, `fail2ban`, `neovim`).
  - Create a new user with sudo privileges.
  - Configure the firewall to allow SSH, HTTP, and HTTPS traffic.
- **Web server setup:**
  - Install Nginx.
  - Create a new Nginx server block for a domain `example.com`.
  - Configure the server block to serve a simple `index.html` file.
- **SSL setup:**
  - Install Certbot and the Nginx plugin.
  - Obtain a free SSL certificate from Let's Encrypt for `example.com`.
  - Configure Nginx to use the SSL certificate and redirect HTTP traffic to HTTPS.

Please generate the complete Ansible playbook as a single block of code. The playbook should be well-commented and follow best practices."
