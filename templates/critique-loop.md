
# Critique Loop Prompt

## Prompt

"Critique the following Ansible playbook for setting up a new Ubuntu server. The playbook should be idempotent and follow best practices.

```yaml
---
- hosts: all
  become: yes
  tasks:
    - name: Update apt cache
      apt:
        update_cache: yes

    - name: Install common packages
      apt:
        name: ['ufw', 'fail2ban', 'neovim']
        state: present

    - name: Enable firewall
      ufw:
        state: enabled
```

Provide feedback on the following aspects:
- **Idempotency:** Is the playbook fully idempotent? If not, what changes are needed?
- **Best Practices:** Does the playbook follow Ansible best practices? Are there any security considerations that have been missed?
- **Readability:** Is the playbook easy to read and understand?
- **Modularity:** Could the playbook be made more modular and reusable?

Please provide specific suggestions for improvement, including code snippets where appropriate."
