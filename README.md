# arch-ansible - Automated Arch Linux Configuration

# Install a base system
Install a minimal Arch Linux base system before using playbook.
Make sure you have `git`, `ansible` and network connectivity (duh!).

# How to run the playbook
After the initial minimal Arch installation:
```bash
git clone https://github.com/itsorphic/arch-ansible.git
cd arch-ansible
vim group_vars/all # Edit the variables as you wish
ansible-playbook -i inventory/localhost playbook.yml [--tags $LIMIT_TO_TAG]
```

**Available tags:**
- network
- base
- firewall
- dotfiles
- shell
- editor
- terminal
- windowmanager
- browsers
- keepass
- sound

# To-Do
- [ ] Dotfiles
- [ ] Customization files for COSMIC.
- [ ] Hacking tooling.
