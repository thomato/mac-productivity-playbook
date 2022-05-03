# Setup
When your run this playbook on a new Mac, make sure to install the prerequisites:

*Install brew*
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

*Install Ansible*
Also, Git may need to be installed to download the playbook.
```
brew install ansible
brew install git
```

*Install Ansible requirements*
```
ansible-galaxy install -r requirements.yml
```

*Fill `vars/local.yml`*
Copy `vars/local.yml.dist` to `vars/local.yml` and change the variables to your choosing.

## Run run run
```
ansible-playbook main.yml --ask-become-pass
```
