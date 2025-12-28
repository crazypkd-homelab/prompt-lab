
# Security Review Prompt

## Prompt

"Please perform a security review of my homelab setup and provide recommendations for improvement.

My setup includes:
- A Proxmox server exposed to the internet via a port-forwarded SSH connection.
- A number of services running in VMs and containers, some of which are accessible from the internet (e.g., a web server, a VPN server).
- Default passwords have been changed, but I'm not sure what other security measures I should be taking.

I'm looking for recommendations on how to secure the following:
- **Proxmox Host:** How can I secure the Proxmox host itself? What are some best practices for SSH security?
- **Network:** How can I secure my network and protect it from external threats?
- **VMs and Containers:** How can I secure the VMs and containers running on my Proxmox host?
- **Web Applications:** What are some common security vulnerabilities in web applications, and how can I protect against them?
- **Data:** How can I protect my data from unauthorized access?

Please provide a checklist of security best practices that I can follow for my homelab."
