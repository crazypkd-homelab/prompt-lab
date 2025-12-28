
# Refactor Code Prompt

## Prompt

"Refactor the following Python script to be more modular and reusable. The script currently has all the logic in a single function.

```python
import requests
import urllib3

def get_proxmox_data():
    urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)

    proxmox_host = '192.168.1.100'
    proxmox_port = 8006
    proxmox_user = 'root@pam'
    proxmox_token_name = 'api-token'
    proxmox_token_value = 'your-api-token'

    headers = {
        'Authorization': f'PVEAPIToken={proxmox_token_name}={proxmox_token_value}',
    }

    url = f'https://{proxmox_host}:{proxmox_port}/api2/json/nodes'
    response = requests.get(url, headers=headers, verify=False)
    response.raise_for_status()
    nodes = response.json()['data']

    for node in nodes:
        print(node['node'])

if __name__ == '__main__':
    get_proxmox_data()
```

The refactored code should have the following structure:
- A `ProxmoxAPI` class that handles the authentication and communication with the Proxmox API.
- A method within the `ProxmoxAPI` class to get the list of nodes.
- A main block that instantiates the `ProxmoxAPI` class and calls the method to get the nodes.

The refactored code should be more organized, easier to test, and reusable in other scripts."
