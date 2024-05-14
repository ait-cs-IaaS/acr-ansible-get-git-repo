# Ansible-Role: acr-ansible-get-git-repo

AIT-CyberRange: Install git and clone repo to remote machine. 


## Requirements

- Debian or Ubuntu 

## Role Variables

```yaml
repo_basepath: /opt/repo
repo_user: root
repo_group: "{{ repo_user }}"
repo_url: https://PAT@github.com/user/repo.git
repo_branch: master
```

## Example Playbook

```yaml
- hosts: all
  roles:
    - acr-ansible-get-git-repo
      vars:
        repo_basepath: /opt/repo
        repo_user: username
        repo_url: https://PAT@github.com/user/repo.git
```

## License

GPL-3.0

## Author

- Lenhard Reuter