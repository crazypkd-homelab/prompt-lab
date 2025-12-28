
# Infrastructure Review Prompt

## Prompt

"Please review my current homelab infrastructure and provide suggestions for improvement.

My current setup consists of:
- A single Proxmox server with 64GB of RAM and 2TB of storage.
- A mix of VMs and LXC containers running various services, including:
  - A pfSense firewall.
  - A Pi-hole DNS server.
  - A Home Assistant instance.
  - A Plex media server.
  - A few development VMs for testing and experimentation.
- A simple, flat network topology with a single VLAN.

I'm looking for feedback on the following areas:
- **Networking:** How can I improve my network security and segmentation? Should I be using VLANs?
- **Storage:** Is my current storage setup adequate? Should I consider using a NAS or a distributed storage solution like Ceph?
- **High Availability:** What are some strategies I can use to improve the availability of my services? Should I consider setting up a Proxmox cluster?
- **Monitoring and Observability:** What tools and techniques can I use to better monitor my infrastructure?

Please provide specific and actionable recommendations that I can implement in my homelab."
